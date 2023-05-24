# Comparing `tmp/graphdatascience-1.6rc1.tar.gz` & `tmp/graphdatascience-1.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdatascience-1.6rc1.tar", last modified: Fri Jan 13 15:50:51 2023, max compression
+gzip compressed data, was "graphdatascience-1.7a1.tar", last modified: Wed May 24 12:08:18 2023, max compression
```

## Comparing `graphdatascience-1.6rc1.tar` & `graphdatascience-1.7a1.tar`

### file list

```diff
@@ -1,116 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.114076 graphdatascience-1.6rc1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      186 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6939 2023-01-13 15:50:51.114076 graphdatascience-1.6rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5637 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:50.994076 graphdatascience-1.6rc1/graphdatascience/
--rw-r--r--   0 root         (0) root         (0)      195 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:50.998076 graphdatascience-1.6rc1/graphdatascience/algo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/algo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/algo/algo_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/algo/algo_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/algo/single_mode_algo_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/call_builder.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/caller_base.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/direct_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:50.998076 graphdatascience-1.6rc1/graphdatascience/error/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/error/__init__.py
--rw-r--r--   0 root         (0) root         (0)      656 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/error/client_only_endpoint.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/error/illegal_attr_checker.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/error/unable_to_connect.py
--rw-r--r--   0 root         (0) root         (0)      290 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/error/uncallable_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.006076 graphdatascience-1.6rc1/graphdatascience/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)      275 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_endpoints.py
--rw-r--r--   0 root         (0) root         (0)    12444 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_entity_ops_runner.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_export_runner.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_object.py
--rw-r--r--   0 root         (0) root         (0)    17090 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_project_runner.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_sample_runner.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph/graph_type_check.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/graph_data_science.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/indirect_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.010076 graphdatascience-1.6rc1/graphdatascience/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/graphsage_model.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/link_prediction_model.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/model.py
--rw-r--r--   0 root         (0) root         (0)      275 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/model_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/model_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/node_classification_model.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/node_regression_model.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/model/pipeline_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.014076 graphdatascience-1.6rc1/graphdatascience/pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/classification_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/lp_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/lp_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/nc_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/nc_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/nr_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/nr_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/pipeline_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/pipeline_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     5472 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/pipeline/training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.014076 graphdatascience-1.6rc1/graphdatascience/query_runner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/arrow_graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)     9260 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/arrow_query_runner.py
--rw-r--r--   0 root         (0) root         (0)    17806 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/cypher_graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)     5102 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/neo4j_query_runner.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/query_runner/query_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.014076 graphdatascience-1.6rc1/graphdatascience/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.018076 graphdatascience-1.6rc1/graphdatascience/resources/cora/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/cora/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109404 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/cora/cora_nodes_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    18041 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/cora/cora_rels_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)     1231 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/cora/serialize_cora.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.022076 graphdatascience-1.6rc1/graphdatascience/resources/imdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42197 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)   246714 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_actors_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    15825 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    94640 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_directors_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)   112462 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl
--rw-r--r--   0 root         (0) root         (0)    64260 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.026076 graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/
--rw-r--r--   0 root         (0) root         (0)   652688 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/edges.pkl
--rw-r--r--   0 root         (0) root         (0)    37310 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/labels.pkl
--rw-r--r--   0 root         (0) root         (0) 64166690 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/node_features.pkl
--rw-r--r--   0 root         (0) root         (0)     3493 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/imdb/serialize_imdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.110076 graphdatascience-1.6rc1/graphdatascience/resources/karate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/karate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      727 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/resources/karate/karate_club_gzip.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.110076 graphdatascience-1.6rc1/graphdatascience/server_version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/server_version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/server_version/compatible_with.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/server_version/server_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.110076 graphdatascience-1.6rc1/graphdatascience/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/system/config_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     2657 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/system/system_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.114076 graphdatascience-1.6rc1/graphdatascience/topological_lp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/topological_lp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/topological_lp/topological_lp_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/topological_lp/topological_lp_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.114076 graphdatascience-1.6rc1/graphdatascience/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/utils/util_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1381 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/utils/util_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/graphdatascience/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:50.994076 graphdatascience-1.6rc1/graphdatascience.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6939 2023-01-13 15:50:50.000000 graphdatascience-1.6rc1/graphdatascience.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4148 2023-01-13 15:50:50.000000 graphdatascience-1.6rc1/graphdatascience.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 15:50:50.000000 graphdatascience-1.6rc1/graphdatascience.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 15:50:50.000000 graphdatascience-1.6rc1/graphdatascience.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       91 2023-01-13 15:50:50.000000 graphdatascience-1.6rc1/graphdatascience.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-13 15:50:50.000000 graphdatascience-1.6rc1/graphdatascience.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 15:50:51.114076 graphdatascience-1.6rc1/requirements/
--rw-r--r--   0 root         (0) root         (0)      111 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-13 15:50:51.114076 graphdatascience-1.6rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1850 2023-01-13 15:49:27.000000 graphdatascience-1.6rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.877512 graphdatascience-1.7a1/graphdatascience/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.877512 graphdatascience-1.7a1/graphdatascience/algo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/algo_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/algo_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/algo/single_mode_algo_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/call_builder.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/caller_base.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.881512 graphdatascience-1.7a1/graphdatascience/error/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      766 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/client_only_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/deprecation_warning.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/endpoint_suggester.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/illegal_attr_checker.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/unable_to_connect.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/error/uncallable_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.881512 graphdatascience-1.7a1/graphdatascience/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_alpha_project_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)    13049 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_entity_ops_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_export_runner.py
+-rw-r--r--   0 root         (0) root         (0)     6689 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_object.py
+-rw-r--r--   0 root         (0) root         (0)    16626 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_project_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_sample_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/graph_type_check.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/nx_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14488 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph/ogb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     8612 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/graph_data_science.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/ignored_server_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.885512 graphdatascience-1.7a1/graphdatascience/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/graphsage_model.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/link_prediction_model.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/model_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/node_classification_model.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/node_regression_model.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/model/pipeline_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.885512 graphdatascience-1.7a1/graphdatascience/pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/classification_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/lp_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/lp_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nc_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nc_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nr_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/nr_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     8211 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/pipeline/training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/query_runner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/arrow_graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)     9319 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/arrow_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/aura_db_arrow_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)    17897 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/cypher_graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)     7477 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/neo4j_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/query_runner/query_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/resources/cora/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109404 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/cora_nodes_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    18041 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/cora_rels_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/cora/serialize_cora.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.889512 graphdatascience-1.7a1/graphdatascience/resources/imdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42197 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)   246714 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_actors_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    15825 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    94640 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directors_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)   112462 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl
+-rw-r--r--   0 root         (0) root         (0)    64260 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.893512 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/
+-rw-r--r--   0 root         (0) root         (0)   652688 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/edges.pkl
+-rw-r--r--   0 root         (0) root         (0)    37310 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/labels.pkl
+-rw-r--r--   0 root         (0) root         (0) 64166690 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/node_features.pkl
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/imdb/serialize_imdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/resources/karate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/karate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/resources/karate/karate_club_gzip.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/server_version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/server_version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/server_version/compatible_with.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/server_version/server_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/system/config_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/system/system_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.965512 graphdatascience-1.7a1/graphdatascience/topological_lp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/topological_lp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/topological_lp/topological_lp_alpha_runner.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/topological_lp/topological_lp_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/graphdatascience/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/utils/util_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/utils/util_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/graphdatascience/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.877512 graphdatascience-1.7a1/graphdatascience.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-24 12:08:18.000000 graphdatascience-1.7a1/graphdatascience.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.873512 graphdatascience-1.7a1/requirements/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/requirements/base/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/requirements/base/base.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/requirements/base/networkx.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/requirements/base/ogb.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:08:18.969512 graphdatascience-1.7a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-24 12:07:06.000000 graphdatascience-1.7a1/setup.py
```

### Comparing `graphdatascience-1.6rc1/LICENSE` & `graphdatascience-1.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/PKG-INFO` & `graphdatascience-1.7a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdatascience
-Version: 1.6rc1
+Version: 1.7a1
 Summary: A Python client for the Neo4j Graph Data Science (GDS) library
 Home-page: https://neo4j.com/product/graph-data-science/
 Author: Neo4j
 Author-email: team-gds@neo4j.org
 License: Apache License 2.0
 Project-URL: Documentation, https://neo4j.com/docs/graph-data-science-client/current/
 Project-URL: Source, https://github.com/neo4j/graph-data-science-client
@@ -16,20 +16,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: ogb
+Provides-Extra: networkx
 License-File: LICENSE
 
 # Neo4j Graph Data Science Client
 
 [![Latest version](https://img.shields.io/pypi/v/graphdatascience)](https://pypi.org/project/graphdatascience/)
 [![PyPI downloads month](https://img.shields.io/pypi/dm/graphdatascience)](https://pypi.org/project/graphdatascience/)
 ![Python versions](https://img.shields.io/pypi/pyversions/graphdatascience)
@@ -105,17 +108,17 @@
 
 The example here assumes using an AuraDS instance.
 For additional examples and extensive documentation of all capabilities, please refer to the [GDS Python Client Manual](https://neo4j.com/docs/graph-data-science-client/current/).
 
 Full end-to-end examples in Jupyter ready-to-run notebooks can be found in the [`examples` source directory](https://github.com/neo4j/graph-data-science-client/tree/main/examples):
 
 * [Machine learning pipelines: Node classification](examples/ml-pipelines-node-classification.ipynb)
-* [Node regression with subgraph and sampling projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
+* [Node Regression with Subgraph and Graph Sample projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
 * [Product recommendations with kNN based on FastRP embeddings](examples/fastrp-and-knn.ipynb)
-* [Exporting from GDS and running GNN with PyG](examples/import-sample-export-gnn.ipynb)
+* [Sampling, Export and Integration with PyG example](examples/import-sample-export-gnn.ipynb)
 * [Load data to a projected graph via graph construction](examples/load-data-via-graph-construction.ipynb)
 * [Heterogeneous Node Classification with HashGNN and Autotuning](https://github.com/neo4j/graph-data-science-client/tree/main/examples/heterogeneous-node-classification-with-hashgnn.ipynb)
 
 
 ## Documentation
 
 The primary source for learning everything about the GDS Python Client is the manual, hosted at https://neo4j.com/docs/graph-data-science-client/current/.
@@ -124,14 +127,15 @@
 
 ## Known limitations
 
 Operations known to not yet work with `graphdatascience`:
 
 * [Numeric utility functions](https://neo4j.com/docs/graph-data-science/current/management-ops/utility-functions/#utility-functions-numeric) (will never be supported)
 * [Cypher on GDS](https://neo4j.com/docs/graph-data-science/current/management-ops/create-cypher-db/) (might be supported in the future)
+* [Projecting graphs using Cypher Aggregation](https://neo4j.com/docs/graph-data-science/current/management-ops/projections/graph-project-cypher-aggregation/) (might be supported in the future)
 
 
 ## License
 
 `graphdatascience` is licensed under the Apache Software License version 2.0.
 All content is copyright © Neo4j Sweden AB.
```

### Comparing `graphdatascience-1.6rc1/README.md` & `graphdatascience-1.7a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 The example here assumes using an AuraDS instance.
 For additional examples and extensive documentation of all capabilities, please refer to the [GDS Python Client Manual](https://neo4j.com/docs/graph-data-science-client/current/).
 
 Full end-to-end examples in Jupyter ready-to-run notebooks can be found in the [`examples` source directory](https://github.com/neo4j/graph-data-science-client/tree/main/examples):
 
 * [Machine learning pipelines: Node classification](examples/ml-pipelines-node-classification.ipynb)
-* [Node regression with subgraph and sampling projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
+* [Node Regression with Subgraph and Graph Sample projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
 * [Product recommendations with kNN based on FastRP embeddings](examples/fastrp-and-knn.ipynb)
-* [Exporting from GDS and running GNN with PyG](examples/import-sample-export-gnn.ipynb)
+* [Sampling, Export and Integration with PyG example](examples/import-sample-export-gnn.ipynb)
 * [Load data to a projected graph via graph construction](examples/load-data-via-graph-construction.ipynb)
 * [Heterogeneous Node Classification with HashGNN and Autotuning](https://github.com/neo4j/graph-data-science-client/tree/main/examples/heterogeneous-node-classification-with-hashgnn.ipynb)
 
 
 ## Documentation
 
 The primary source for learning everything about the GDS Python Client is the manual, hosted at https://neo4j.com/docs/graph-data-science-client/current/.
@@ -94,14 +94,15 @@
 
 ## Known limitations
 
 Operations known to not yet work with `graphdatascience`:
 
 * [Numeric utility functions](https://neo4j.com/docs/graph-data-science/current/management-ops/utility-functions/#utility-functions-numeric) (will never be supported)
 * [Cypher on GDS](https://neo4j.com/docs/graph-data-science/current/management-ops/create-cypher-db/) (might be supported in the future)
+* [Projecting graphs using Cypher Aggregation](https://neo4j.com/docs/graph-data-science/current/management-ops/projections/graph-project-cypher-aggregation/) (might be supported in the future)
 
 
 ## License
 
 `graphdatascience` is licensed under the Apache Software License version 2.0.
 All content is copyright © Neo4j Sweden AB.
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/algo/algo_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/algo/algo_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/algo/algo_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/algo/algo_proc_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from abc import ABC
 from typing import Any, Dict, Tuple
 
 from pandas import DataFrame, Series
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..graph.graph_object import Graph
 from ..graph.graph_type_check import graph_type_check
 from ..model.graphsage_model import GraphSageModel
 
 
-class AlgoProcRunner(CallerBase, IllegalAttrChecker, ABC):
+class AlgoProcRunner(IllegalAttrChecker, ABC):
     @graph_type_check
     def _run_procedure(self, G: Graph, config: Dict[str, Any], with_logging: bool = True) -> DataFrame:
         query = f"CALL {self._namespace}($graph_name, $config)"
 
         params: Dict[str, Any] = {}
         params["graph_name"] = G.name()
         params["config"] = config
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/graph/graph_entity_ops_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_entity_ops_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from functools import reduce
 from typing import Any, Dict, List, Type, Union
 
 import pandas as pd
 from pandas import DataFrame, Series
 
+from ..error.illegal_attr_checker import IllegalAttrChecker
+from ..error.uncallable_namespace import UncallableNamespace
+from ..query_runner.query_runner import QueryRunner
+from ..server_version.compatible_with import compatible_with
+from ..server_version.server_version import ServerVersion
 from ..utils.util_proc_runner import UtilProcRunner
 from .graph_object import Graph
 from .graph_type_check import graph_type_check
-from graphdatascience.caller_base import CallerBase
-from graphdatascience.error.illegal_attr_checker import IllegalAttrChecker
-from graphdatascience.error.uncallable_namespace import UncallableNamespace
-from graphdatascience.query_runner.query_runner import QueryRunner
-from graphdatascience.server_version.compatible_with import compatible_with
-from graphdatascience.server_version.server_version import ServerVersion
 
 Strings = Union[str, List[str]]
 
 
 class TopologyDataFrame(DataFrame):
     @property
     def _constructor(self) -> "Type[TopologyDataFrame]":
@@ -29,15 +28,15 @@
         for rel_type, indices in gb.groups.items():
             one_rel_df = self.take(indices)
             output[str(rel_type)] = [list(one_rel_df["sourceNodeId"]), list(one_rel_df["targetNodeId"])]
 
         return output
 
 
-class GraphEntityOpsBaseRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class GraphEntityOpsBaseRunner(UncallableNamespace, IllegalAttrChecker):
     def __init__(self, query_runner: QueryRunner, namespace: str, server_version: ServerVersion):
         super().__init__(query_runner, namespace, server_version)
         self._util_proc_runner = UtilProcRunner(query_runner, "gds.util", server_version)
 
     @graph_type_check
     def _handle_properties(
         self,
@@ -166,14 +165,35 @@
         elif not separate_property_columns and "propertyValue" not in result.keys():
             result = result.melt(id_vars=["sourceNodeId", "targetNodeId", "relationshipType"]).rename(
                 columns={"variable": "relationshipProperty", "value": "propertyValue"}
             )
 
         return result
 
+    @compatible_with("write", min_inclusive=ServerVersion(2, 4, 0))
+    @graph_type_check
+    def write(
+        self,
+        G: Graph,
+        relationship_type: str,
+        relationship_properties: List[str],
+        **config: Any,
+    ) -> "Series[Any]":
+        self._namespace += ".write"
+
+        query = f"CALL {self._namespace}($graph_name, $relationship_type, $relationship_properties, $config)"
+        params = {
+            "graph_name": G.name(),
+            "relationship_type": relationship_type,
+            "relationship_properties": relationship_properties,
+            "config": config,
+        }
+
+        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+
 
 class GraphRelationshipRunner(GraphEntityOpsBaseRunner):
     @compatible_with("write", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def write(self, G: Graph, relationship_type: str, relationship_property: str = "", **config: Any) -> "Series[Any]":
         self._namespace += ".write"
         query = f"CALL {self._namespace}($graph_name, $relationship_type, $relationship_property, $config)"
@@ -183,15 +203,15 @@
             "relationship_property": relationship_property,
             "config": config,
         }
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
 
-class ToUndirectedRunner(CallerBase, IllegalAttrChecker):
+class ToUndirectedRunner(IllegalAttrChecker):
     def _run_procedure(
         self, G: Graph, query: str, relationship_type: str, mutate_relationship_type: str, **config: Any
     ) -> "Series[Any]":
         actual_config = {
             **config,
             "relationshipType": relationship_type,
             "mutateRelationshipType": mutate_relationship_type,
@@ -225,14 +245,16 @@
         params = {
             "graph_name": G.name(),
             "relationship_type": relationship_type,
         }
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
+
+class GraphRelationshipsBetaRunner(GraphEntityOpsBaseRunner):
     @compatible_with("stream", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def stream(self, G: Graph, relationship_types: List[str] = ["*"], **config: Any) -> TopologyDataFrame:
         self._namespace += ".stream"
         query = f"CALL {self._namespace}($graph_name, $relationship_types, $config)"
 
         params = {"graph_name": G.name(), "relationship_types": relationship_types, "config": config}
@@ -242,15 +264,15 @@
     @property
     @compatible_with("toUndirected", min_inclusive=ServerVersion(2, 3, 0))
     def toUndirected(self) -> ToUndirectedRunner:
         self._namespace += ".toUndirected"
         return ToUndirectedRunner(self._query_runner, self._namespace, self._server_version)
 
 
-class GraphPropertyRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class GraphPropertyRunner(UncallableNamespace, IllegalAttrChecker):
     @compatible_with("stream", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def stream(
         self,
         G: Graph,
         graph_property: str,
         **config: Any,
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/graph/graph_export_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_export_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict
 
 from pandas import Series
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
+from ..error.uncallable_namespace import UncallableNamespace
 from .graph_object import Graph
 from .graph_type_check import graph_type_check
 
 
-class GraphExportCsvRunner(CallerBase, IllegalAttrChecker):
+class GraphExportCsvRunner(IllegalAttrChecker):
     # TODO: Add an integration test for this call.
     def __call__(self, G: Graph, **config: Any) -> "Series[Any]":
         return self._export_call(G, config)
 
     @graph_type_check
     def _export_call(self, G: Graph, config: Dict[str, Any]) -> "Series[Any]":
         query = f"CALL {self._namespace}($graph_name, $config)"
@@ -23,15 +23,23 @@
     @graph_type_check
     def estimate(self, G: Graph, **config: Any) -> "Series[Any]":
         self._namespace += ".estimate"
 
         return self._export_call(G, config)
 
 
-class GraphExportRunner(CallerBase, IllegalAttrChecker):
+class GraphExportCsvEndpoints(UncallableNamespace, IllegalAttrChecker):
+    @property
+    def csv(self) -> GraphExportCsvRunner:
+        self._namespace += ".csv"
+
+        return GraphExportCsvRunner(self._query_runner, self._namespace, self._server_version)
+
+
+class GraphExportRunner(IllegalAttrChecker):
     def __call__(self, G: Graph, **config: Any) -> "Series[Any]":
         return self._export_call(G, config)
 
     @graph_type_check
     def _export_call(self, G: Graph, config: Dict[str, Any]) -> "Series[Any]":
         query = f"CALL {self._namespace}($graph_name, $config)"
         params = {"graph_name": G.name(), "config": config}
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/graph/graph_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_proc_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,156 @@
-import os
-from importlib.resources import path
-from typing import Any, Dict, List, Optional, Tuple, Union
+import pathlib
+import sys
+from logging import warning
+from typing import Any, ContextManager, Dict, List, Optional, Union
 
 import pandas as pd
 from multimethod import multimethod
 from pandas import DataFrame, Series, read_pickle
 
-from ..caller_base import CallerBase
 from ..error.client_only_endpoint import client_only_endpoint
+from ..error.deprecation_warning import deprecation_warning
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
-from .graph_export_runner import GraphExportRunner
-from .graph_object import Graph
-from .graph_project_runner import GraphProjectRunner
-from .graph_sample_runner import GraphSampleRunner
-from graphdatascience.graph.graph_entity_ops_runner import (
+from .graph_alpha_proc_runner import GraphAlphaProcRunner
+from .graph_entity_ops_runner import (
     GraphElementPropertyRunner,
-    GraphLabelRunner,
     GraphNodePropertiesRunner,
-    GraphPropertyRunner,
     GraphRelationshipPropertiesRunner,
     GraphRelationshipRunner,
     GraphRelationshipsRunner,
 )
-from graphdatascience.graph.graph_type_check import (
-    graph_type_check,
-    graph_type_check_optional,
-)
+from .graph_export_runner import GraphExportRunner
+from .graph_object import Graph
+from .graph_project_runner import GraphProjectRunner
+from .graph_sample_runner import GraphSampleRunner
+from .graph_type_check import graph_type_check, graph_type_check_optional
+from .ogb_loader import OGBLLoader, OGBNLoader
 
 Strings = Union[str, List[str]]
 
 
-class GraphProcRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class GraphProcRunner(UncallableNamespace, IllegalAttrChecker):
+    @staticmethod
+    def _path(package: str, resource: str) -> ContextManager[pathlib.Path]:
+        if sys.version_info >= (3, 9):
+            import os.path
+            from importlib.resources import as_file, files
+
+            return as_file(files(package) / os.path.normpath(resource))
+        else:
+            from importlib.resources import path
+
+            return path(package, resource)
+
     @client_only_endpoint("gds.graph")
     def load_cora(self, graph_name: str = "cora", undirected: bool = False) -> Graph:
-        with path("graphdatascience.resources.cora", "cora_nodes_gzip.pkl") as nodes_resource:
+        with self._path("graphdatascience.resources.cora", "cora_nodes_gzip.pkl") as nodes_resource:
             nodes = read_pickle(nodes_resource, compression="gzip")
 
-        with path("graphdatascience.resources.cora", "cora_rels_gzip.pkl") as rels_resource:
+        with self._path("graphdatascience.resources.cora", "cora_rels_gzip.pkl") as rels_resource:
             rels = read_pickle(rels_resource, compression="gzip")
 
         self._namespace = "gds.alpha.graph"
+        alpha_proc_runner = GraphAlphaProcRunner(self._query_runner, self._namespace, self._server_version)
 
         undirected_relationship_types = ["*"] if undirected else []
 
-        return self.construct(graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types)
+        return alpha_proc_runner.construct(
+            graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types
+        )
 
     @client_only_endpoint("gds.graph")
     def load_karate_club(self, graph_name: str = "karate_club", undirected: bool = False) -> Graph:
         nodes = pd.DataFrame({"nodeId": range(1, 35)})
         nodes["labels"] = "Person"
 
-        with path("graphdatascience.resources.karate", "karate_club_gzip.pkl") as rels_resource:
+        with self._path("graphdatascience.resources.karate", "karate_club_gzip.pkl") as rels_resource:
             rels = read_pickle(rels_resource, compression="gzip")
 
         self._namespace = "gds.alpha.graph"
+        alpha_proc_runner = GraphAlphaProcRunner(self._query_runner, self._namespace, self._server_version)
 
         undirected_relationship_types = ["*"] if undirected else []
 
-        return self.construct(graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types)
+        return alpha_proc_runner.construct(
+            graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types
+        )
 
     @client_only_endpoint("gds.graph")
     def load_imdb(self, graph_name: str = "imdb", undirected: bool = True) -> Graph:
         if self._server_version < ServerVersion(2, 3, 0):
             raise ValueError("The IMDB dataset loading is only supported by GDS 2.3 or later.")
 
-        with path("graphdatascience.resources.imdb", "imdb_movies_with_genre_gzip.pkl") as nodes_resource:
+        with self._path("graphdatascience.resources.imdb", "imdb_movies_with_genre_gzip.pkl") as nodes_resource:
             movies_with_genre = read_pickle(nodes_resource, compression="gzip")
-        with path("graphdatascience.resources.imdb", "imdb_movies_without_genre_gzip.pkl") as nodes_resource:
+        with self._path("graphdatascience.resources.imdb", "imdb_movies_without_genre_gzip.pkl") as nodes_resource:
             movies_without_genre = read_pickle(nodes_resource, compression="gzip")
-        with path("graphdatascience.resources.imdb", "imdb_actors_gzip.pkl") as nodes_resource:
+        with self._path("graphdatascience.resources.imdb", "imdb_actors_gzip.pkl") as nodes_resource:
             actors = read_pickle(nodes_resource, compression="gzip")
-        with path("graphdatascience.resources.imdb", "imdb_directors_gzip.pkl") as nodes_resource:
+        with self._path("graphdatascience.resources.imdb", "imdb_directors_gzip.pkl") as nodes_resource:
             directors = read_pickle(nodes_resource, compression="gzip")
 
-        with path("graphdatascience.resources.imdb", "imdb_acted_in_rels_gzip.pkl") as rels_resource:
+        with self._path("graphdatascience.resources.imdb", "imdb_acted_in_rels_gzip.pkl") as rels_resource:
             acted_in_rels = read_pickle(rels_resource, compression="gzip")
-        with path("graphdatascience.resources.imdb", "imdb_directed_in_rels_gzip.pkl") as rels_resource:
+        with self._path("graphdatascience.resources.imdb", "imdb_directed_in_rels_gzip.pkl") as rels_resource:
             directed_in_rels = read_pickle(rels_resource, compression="gzip")
 
         self._namespace = "gds.alpha.graph"
+        alpha_proc_runner = GraphAlphaProcRunner(self._query_runner, self._namespace, self._server_version)
 
         nodes = [movies_with_genre, movies_without_genre, actors, directors]
         rels = [acted_in_rels, directed_in_rels]
 
         # Default undirected which matches raw data
         undirected_relationship_types = ["*"] if undirected else []
 
-        return self.construct(graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types)
+        return alpha_proc_runner.construct(
+            graph_name, nodes, rels, undirected_relationship_types=undirected_relationship_types
+        )
+
+    @property
+    def sample(self) -> GraphSampleRunner:
+        self._namespace += ".sample"
+        return GraphSampleRunner(self._query_runner, self._namespace, self._server_version)
+
+    @property
+    def networkx(self):  # type: ignore
+        try:
+            from .nx_loader import NXLoader
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "This feature requires NetworkX support. "
+                "You can add NetworkX support by running `pip install graphdatascience[networkx]`"
+            )
+
+        self._namespace += ".networkx"
+        return NXLoader(self._query_runner, self._namespace, self._server_version)
 
     @property
     def project(self) -> GraphProjectRunner:
         self._namespace += ".project"
         return GraphProjectRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
     def export(self) -> GraphExportRunner:
         self._namespace += ".export"
         return GraphExportRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
-    def sample(self) -> GraphSampleRunner:
-        self._namespace += ".sample"
-        return GraphSampleRunner(self._query_runner, self._namespace, self._server_version)
+    def ogbn(self) -> OGBNLoader:
+        self._namespace += ".ogbn"
+        return OGBNLoader(self._query_runner, self._namespace, self._server_version)
+
+    @property
+    def ogbl(self) -> OGBLLoader:
+        self._namespace += ".ogbl"
+        return OGBLLoader(self._query_runner, self._namespace, self._server_version)
 
     @graph_type_check
     def drop(
         self,
         G: Graph,
         failIfMissing: bool = False,
         dbName: str = "",
@@ -150,15 +192,17 @@
             query = "CALL gds.graph.list()"
             params = {}
 
         return self._query_runner.run_query(query, params)
 
     @client_only_endpoint("gds.graph")
     def get(self, graph_name: str) -> Graph:
-        result = self._query_runner.run_query(f"CALL gds.graph.list('{graph_name}') YIELD graphName")
+        result = self._query_runner.run_query(
+            f"CALL gds.graph.list('{graph_name}') YIELD graphName", custom_error=False
+        )
         if len(result["graphName"]) == 0:
             raise ValueError(
                 f"No projected graph named '{graph_name}' exists in current database '{self._query_runner.database()}'"
             )
 
         return Graph(graph_name, self._query_runner, self._server_version)
 
@@ -206,24 +250,15 @@
         return GraphRelationshipRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
     def relationships(self) -> GraphRelationshipsRunner:
         self._namespace += ".relationships"
         return GraphRelationshipsRunner(self._query_runner, self._namespace, self._server_version)
 
-    @property
-    def graphProperty(self) -> GraphPropertyRunner:
-        self._namespace += ".graphProperty"
-        return GraphPropertyRunner(self._query_runner, self._namespace, self._server_version)
-
-    @property
-    def nodeLabel(self) -> GraphLabelRunner:
-        self._namespace += ".nodeLabel"
-        return GraphLabelRunner(self._query_runner, self._namespace, self._server_version)
-
+    @deprecation_warning("gds.graph.nodeProperties.stream", ServerVersion(2, 3, 0))
     def streamNodeProperties(
         self,
         G: Graph,
         node_properties: List[str],
         node_labels: Strings = ["*"],
         separate_property_columns: bool = False,
         **config: Any,
@@ -241,25 +276,27 @@
         elif not separate_property_columns and "propertyValue" not in result.keys():
             result = result.melt(id_vars=["nodeId"]).rename(
                 columns={"variable": "nodeProperty", "value": "propertyValue"}
             )
 
         return result
 
+    @deprecation_warning("gds.graph.nodeProperty.stream", ServerVersion(2, 3, 0))
     def streamNodeProperty(
         self,
         G: Graph,
         node_properties: str,
         node_labels: Strings = ["*"],
         **config: Any,
     ) -> DataFrame:
         self._namespace += ".streamNodeProperty"
 
         return self._handle_properties(G, node_properties, node_labels, config)
 
+    @deprecation_warning("gds.graph.relationshipProperties.stream", ServerVersion(2, 3, 0))
     def streamRelationshipProperties(
         self,
         G: Graph,
         relationship_properties: List[str],
         relationship_types: Strings = ["*"],
         separate_property_columns: bool = False,
         **config: Any,
@@ -281,36 +318,39 @@
         elif not separate_property_columns and "propertyValue" not in result.keys():
             result = result.melt(id_vars=["sourceNodeId", "targetNodeId", "relationshipType"]).rename(
                 columns={"variable": "relationshipProperty", "value": "propertyValue"}
             )
 
         return result
 
+    @deprecation_warning("gds.graph.relationshipProperty.stream", ServerVersion(2, 3, 0))
     def streamRelationshipProperty(
         self,
         G: Graph,
         relationship_properties: str,
         relationship_types: Strings = ["*"],
         **config: Any,
     ) -> DataFrame:
         self._namespace += ".streamRelationshipProperty"
 
         return self._handle_properties(G, relationship_properties, relationship_types, config)
 
+    @deprecation_warning("gds.graph.nodeProperties.write", ServerVersion(2, 3, 0))
     def writeNodeProperties(
         self,
         G: Graph,
         node_properties: List[str],
         node_labels: Strings = ["*"],
         **config: Any,
     ) -> "Series[Any]":
         self._namespace += ".writeNodeProperties"
 
         return self._handle_properties(G, node_properties, node_labels, config).squeeze()  # type: ignore
 
+    @deprecation_warning("gds.graph.relationship.write", ServerVersion(2, 3, 0))
     def writeRelationship(
         self,
         G: Graph,
         relationship_type: str,
         relationship_property: str = "",
         **config: Any,
     ) -> "Series[Any]":
@@ -328,14 +368,15 @@
 
     @multimethod
     def removeNodeProperties(self) -> None:
         ...
 
     @removeNodeProperties.register
     @graph_type_check
+    @deprecation_warning("gds.graph.nodeProperties.drop", ServerVersion(2, 3, 0))
     def _(
         self,
         G: Graph,
         node_properties: List[str],
         **config: Any,
     ) -> Series:  # type: ignore
         self._namespace += ".removeNodeProperties"
@@ -347,92 +388,33 @@
             "config": config,
         }
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
     @removeNodeProperties.register
     @compatible_with("removeNodeProperties", max_exclusive=ServerVersion(2, 1, 0))
+    @deprecation_warning("gds.graph.nodeProperties.drop", ServerVersion(2, 3, 0))
     @graph_type_check
     def _(
         self,
         G: Graph,
         node_properties: List[str],
         node_labels: Strings,
         **config: Any,
     ) -> Series:  # type: ignore
         self._namespace += ".removeNodeProperties"
 
         return self._handle_properties(G, node_properties, node_labels, config).squeeze()  # type: ignore
 
+    @deprecation_warning("gds.graph.relationships.drop", ServerVersion(2, 3, 0))
     @graph_type_check
     def deleteRelationships(self, G: Graph, relationship_type: str) -> "Series[Any]":
+        warning("Deprecated in favor of `gds.relationships.drop`")
         self._namespace += ".deleteRelationships"
 
         query = f"CALL {self._namespace}($graph_name, $relationship_type)"
         params = {
             "graph_name": G.name(),
             "relationship_type": relationship_type,
         }
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
-
-    def generate(
-        self, graph_name: str, node_count: int, average_degree: int, **config: Any
-    ) -> Tuple[Graph, "Series[Any]"]:
-        self._namespace += ".generate"
-
-        query = f"CALL {self._namespace}($graph_name, $node_count, $average_degree, $config)"
-        params = {
-            "graph_name": graph_name,
-            "node_count": node_count,
-            "average_degree": average_degree,
-            "config": config,
-        }
-
-        result = self._query_runner.run_query(query, params).squeeze()
-
-        return Graph(graph_name, self._query_runner, self._server_version), result
-
-    @client_only_endpoint("gds.alpha.graph")
-    @compatible_with("construct", min_inclusive=ServerVersion(2, 1, 0))
-    def construct(
-        self,
-        graph_name: str,
-        nodes: Union[DataFrame, List[DataFrame]],
-        relationships: Union[DataFrame, List[DataFrame]],
-        concurrency: int = 4,
-        undirected_relationship_types: Optional[List[str]] = None,
-    ) -> Graph:
-        nodes = nodes if isinstance(nodes, List) else [nodes]
-        relationships = relationships if isinstance(relationships, List) else [relationships]
-
-        errors = []
-
-        exists = self._query_runner.run_query(f"CALL gds.graph.exists('{graph_name}') YIELD exists").squeeze()
-
-        # compare against True as (1) unit tests return None here and (2) numpys True does not work with `is True`.
-        if exists == True:  # noqa: E712
-            errors.append(
-                f"Graph '{graph_name}' already exists. Please drop the existing graph or use a different name."
-            )
-
-        for idx, node_df in enumerate(nodes):
-            if "nodeId" not in node_df.columns.values:
-                errors.append(f"Node dataframe at index {idx} needs to contain a 'nodeId' column.")
-
-        for idx, rel_df in enumerate(relationships):
-            for expected_col in ["sourceNodeId", "targetNodeId"]:
-                if expected_col not in rel_df.columns.values:
-                    errors.append(f"Relationship dataframe at index {idx} needs to contain a '{expected_col}' column.")
-
-        if self._server_version < ServerVersion(2, 3, 0) and undirected_relationship_types:
-            errors.append("The parameter 'undirected_relationship_types' is only supported since GDS 2.3.0.")
-
-        if len(errors) > 0:
-            raise ValueError(os.linesep.join(errors))
-
-        constructor = self._query_runner.create_graph_constructor(
-            graph_name, concurrency, undirected_relationship_types
-        )
-        constructor.run(nodes, relationships)
-
-        return Graph(graph_name, self._query_runner, self._server_version)
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/graph/graph_project_runner.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_project_runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from .graph_object import Graph
 from .graph_type_check import from_graph_type_check
 
 
-class GraphProjectRunner(CallerBase, IllegalAttrChecker):
+class GraphProjectRunner(IllegalAttrChecker):
     def __call__(
         self, graph_name: str, node_spec: Any, relationship_spec: Any, **config: Any
     ) -> Tuple[Graph, "Series[Any]"]:
         result = self._query_runner.run_query_with_logging(
             f"CALL {self._namespace}($graph_name, $node_spec, $relationship_spec, $config)",
             {
                 "graph_name": graph_name,
@@ -20,31 +19,33 @@
                 "relationship_spec": relationship_spec,
                 "config": config,
             },
         ).squeeze()
 
         return Graph(graph_name, self._query_runner, self._server_version), result
 
-    def estimate(self, node_spec: Any, relationship_spec: Any, **config: Any) -> "Series[Any]":
+    def estimate(self, node_projection: Any, relationship_projection: Any, **config: Any) -> "Series[Any]":
         self._namespace += ".estimate"
         result = self._query_runner.run_query(
             f"CALL {self._namespace}($node_spec, $relationship_spec, $config)",
             {
-                "node_spec": node_spec,
-                "relationship_spec": relationship_spec,
+                "node_spec": node_projection,
+                "relationship_spec": relationship_projection,
                 "config": config,
             },
         )
 
         return result.squeeze()  # type: ignore
 
     @property
     def cypher(self) -> "GraphProjectRunner":
         return GraphProjectRunner(self._query_runner, self._namespace + ".cypher", self._server_version)
 
+
+class GraphProjectBetaRunner(IllegalAttrChecker):
     @from_graph_type_check
     def subgraph(
         self,
         graph_name: str,
         from_G: Graph,
         node_filter: str,
         relationship_filter: str,
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/graph/graph_type_check.py` & `graphdatascience-1.7a1/graphdatascience/graph/graph_type_check.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/graph_data_science.py` & `graphdatascience-1.7a1/graphdatascience/graph_data_science.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import warnings
 from typing import Any, Dict, Optional, Tuple, Type, TypeVar, Union
 
 from neo4j import Driver, GraphDatabase
 from pandas import DataFrame, Series
 
-from .call_builder import CallBuilder
-from .direct_endpoints import DirectEndpoints
+from .call_builder import IndirectCallBuilder
+from .endpoints import AlphaEndpoints, BetaEndpoints, DirectEndpoints
 from .error.unable_to_connect import UnableToConnectError
 from .error.uncallable_namespace import UncallableNamespace
 from .query_runner.arrow_query_runner import ArrowQueryRunner
 from .query_runner.neo4j_query_runner import Neo4jQueryRunner
 from .query_runner.query_runner import QueryRunner
 from .server_version.server_version import ServerVersion
 from .version import __version__
+from graphdatascience.query_runner.aura_db_arrow_query_runner import (
+    AuraDbArrowQueryRunner,
+    AuraDbConnectionInfo,
+)
 
 GDS = TypeVar("GDS", bound="GraphDataScience")
 
 
 class GraphDataScience(DirectEndpoints, UncallableNamespace):
+    """
+    Primary API class for the Neo4j Graph Data Science Python Client.
+    Always bind this object to a variable called `gds`.
+    """
+
     _AURA_DS_PROTOCOL = "neo4j+s"
 
     def __init__(
         self,
         endpoint: Union[str, Driver, QueryRunner],
         auth: Optional[Tuple[str, str]] = None,
         aura_ds: bool = False,
         database: Optional[str] = None,
         arrow: bool = True,
         arrow_disable_server_verification: bool = True,
         arrow_tls_root_certs: Optional[bytes] = None,
+        aura_db_connection_info: Optional[AuraDbConnectionInfo] = None,
     ):
         """
+        Construct a new GraphDataScience object.
+
         Parameters
         ----------
         endpoint : Union[str, Driver, QueryRunner]
-            The Neo4j endpoint to connect to
+            The Neo4j endpoint to connect to. Most commonly, this is a Bolt connection URI.
         auth : Optional[Tuple[str, str]], default None
             A username, password pair for database authentication.
         aura_ds : bool, default False
             A flag that indicates that that the client is used to connect
             to a Neo4j Aura instance.
         database: Optional[str], default None
             The Neo4j database to query against.
@@ -54,23 +66,15 @@
             Arrow Flight server.
         """
 
         if isinstance(endpoint, str):
             self._config: Dict[str, Any] = {"user_agent": f"neo4j-graphdatascience-v{__version__}"}
 
             if aura_ds:
-                protocol = endpoint.split(":")[0]
-                if not protocol == self._AURA_DS_PROTOCOL:
-                    raise ValueError(
-                        f"AuraDS requires using the '{self._AURA_DS_PROTOCOL}' protocol ('{protocol}' was provided)"
-                    )
-
-                self._config["max_connection_lifetime"] = 60 * 8  # 8 minutes
-                self._config["keep_alive"] = True
-                self._config["max_connection_pool_size"] = 50
+                self._configure_aura(endpoint, self._config)
 
             driver = GraphDatabase.driver(endpoint, auth=auth, **self._config)
 
             self._query_runner = Neo4jQueryRunner(driver, auto_close=True)
 
         elif isinstance(endpoint, QueryRunner):
             if arrow:
@@ -82,29 +86,31 @@
             driver = endpoint
             self._query_runner = Neo4jQueryRunner(driver, auto_close=False)
 
         if database:
             self._query_runner.set_database(database)
 
         try:
-            server_version_string = self._query_runner.run_query("RETURN gds.version()").squeeze()
+            server_version_string = self._query_runner.run_query("RETURN gds.version()", custom_error=False).squeeze()
         except Exception as e:
             raise UnableToConnectError(e)
         finally:
             # Some Python versions appear to not call __del__ of self._query_runner when an exception
             # is raised, so we have to close the driver manually.
             if isinstance(endpoint, str):
                 driver.close()
 
         self._server_version = ServerVersion.from_string(server_version_string)
         self._query_runner.set_server_version(self._server_version)
 
         if arrow and self._server_version >= ServerVersion(2, 1, 0):
             try:
-                arrow_info: "Series[Any]" = self._query_runner.run_query("CALL gds.debug.arrow()").squeeze()
+                arrow_info: "Series[Any]" = self._query_runner.run_query(
+                    "CALL gds.debug.arrow()", custom_error=False
+                ).squeeze()
                 listen_address: str = arrow_info.get(
                     "advertisedListenAddress", arrow_info["listenAddress"]
                 )  # type: ignore
                 if arrow_info["running"]:
                     self._query_runner = ArrowQueryRunner(
                         listen_address,
                         self._query_runner,
@@ -119,40 +125,98 @@
                 # TODO: Remove this check when AuraDS gets arrow support.
                 if (
                     "There is no procedure with the name `gds.debug.arrow` "
                     "registered for this database instance." not in str(e)
                 ):
                     warnings.warn(f"Could not initialize GDS Flight Server client: {e}")
 
+        if aura_db_connection_info:
+            if self._server_version >= ServerVersion(2, 4, 0):
+                self._query_runner = AuraDbArrowQueryRunner(self._query_runner, aura_db_connection_info)
+            else:
+                warnings.warn(
+                    f"AuraDB connection info was provided but GDS version {self._server_version} \
+                        does not support connecting to AuraDB"
+                )
+
         super().__init__(self._query_runner, "gds", self._server_version)
 
-    def __getattr__(self, attr: str) -> CallBuilder:
-        return CallBuilder(self._query_runner, f"gds.{attr}", self._server_version)
+    @property
+    def alpha(self) -> AlphaEndpoints:
+        return AlphaEndpoints(self._query_runner, "gds.alpha", self._server_version)
+
+    @property
+    def beta(self) -> BetaEndpoints:
+        return BetaEndpoints(self._query_runner, "gds.beta", self._server_version)
+
+    def __getattr__(self, attr: str) -> IndirectCallBuilder:
+        return IndirectCallBuilder(self._query_runner, f"gds.{attr}", self._server_version)
 
     def set_database(self, database: str) -> None:
         self._query_runner.set_database(database)
 
     def database(self) -> Optional[str]:
         return self._query_runner.database()
 
     def run_cypher(
         self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
     ) -> DataFrame:
+        """
+        Run a Cypher query
+
+        Parameters
+        ----------
+        query: str
+            the Cypher query
+        params: Dict[str, Any]
+            parameters to the query
+        database: str
+            the database on which to run the query
+
+        Returns
+        -------
+        The query result as a DataFrame
+        """
         qr = self._query_runner
 
-        # The Arrow query runner should not be used to execute arbitary Cypher.
+        # The Arrow query runner should not be used to execute arbitrary Cypher
         if isinstance(self._query_runner, ArrowQueryRunner):
             qr = self._query_runner.fallback_query_runner()
 
-        return qr.run_query(query, params, database)
+        return qr.run_query(query, params, database, False)
 
     def driver_config(self) -> Dict[str, Any]:
         return self._config
 
     @classmethod
     def from_neo4j_driver(
-        cls: Type[GDS], driver: Driver, auth: Optional[Tuple[str, str]] = None, arrow: bool = True
+        cls: Type[GDS],
+        driver: Driver,
+        auth: Optional[Tuple[str, str]] = None,
+        database: Optional[str] = None,
+        arrow: bool = True,
+        arrow_disable_server_verification: bool = True,
+        arrow_tls_root_certs: Optional[bytes] = None,
     ) -> "GraphDataScience":
-        return cls(driver, auth=auth, arrow=arrow)
+        return cls(
+            driver,
+            auth=auth,
+            database=database,
+            arrow=arrow,
+            arrow_disable_server_verification=arrow_disable_server_verification,
+            arrow_tls_root_certs=arrow_tls_root_certs,
+        )
 
     def close(self) -> None:
         self._query_runner.close()
+
+    @classmethod
+    def _configure_aura(cls, uri: str, config: Dict[str, Any]) -> None:
+        protocol = uri.split(":")[0]
+        if not protocol == cls._AURA_DS_PROTOCOL:
+            raise ValueError(
+                f"AuraDS requires using the '{cls._AURA_DS_PROTOCOL}' protocol ('{protocol}' was provided)"
+            )
+
+        config["max_connection_lifetime"] = 60 * 8  # 8 minutes
+        config["keep_alive"] = True
+        config["max_connection_pool_size"] = 50
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/classification_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/classification_training_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,60 @@
 from abc import ABC
 from typing import Any
 
 from pandas import Series
 
+from ..server_version.server_version import ServerVersion
 from .training_pipeline import MODEL_TYPE, TrainingPipeline
 
 
 class ClassificationTrainingPipeline(TrainingPipeline[MODEL_TYPE], ABC):
     def addLogisticRegression(self, **config: Any) -> "Series[Any]":
+        """
+        Add a logistic regression model candidate to the pipeline.
+
+        Args:
+            **config: The configuration for the logistic regression model.
+
+        Returns:
+            The result of the query.
+        """
         query = f"{self._query_prefix()}addLogisticRegression($pipeline_name, $config)"
         params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
     def addRandomForest(self, **config: Any) -> "Series[Any]":
-        query_prefix = self._query_prefix().replace("beta", "alpha")
+        """
+        Add a random forest model candidate to the pipeline.
+
+        Args:
+            **config: The configuration for the random forest model.
+
+        Returns:
+            The result of the query.
+
+        """
+        query_prefix = self._query_prefix()
+        if self._server_version < ServerVersion(2, 4, 0):
+            query_prefix = self._query_prefix().replace("beta", "alpha")
         query = f"{query_prefix}addRandomForest($pipeline_name, $config)"
         params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
     def addMLP(self, **config: Any) -> "Series[Any]":
+        """
+        Add a multi-layer perceptron model candidate to the pipeline.
+
+        Args:
+            **config: The configuration for the multi-layer perceptron model.
+
+        Returns:
+            The result of the query.
+
+        """
         query_prefix = self._query_prefix().replace("beta", "alpha")
         query = f"{query_prefix}addMLP($pipeline_name, $config)"
         params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/lp_pipeline_create_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/lp_pipeline_create_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from .lp_training_pipeline import LPTrainingPipeline
 
 
-class LPPipelineCreateRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class LPPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
     def create(self, name: str) -> Tuple[LPTrainingPipeline, "Series[Any]"]:
         self._namespace += ".create"
 
         query = f"CALL {self._namespace}($name)"
         params = {"name": name}
         result = self._query_runner.run_query(query, params).squeeze()
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/lp_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/lp_training_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,47 @@
 
 from ..model.link_prediction_model import LPModel
 from ..query_runner.query_runner import QueryRunner
 from .classification_training_pipeline import ClassificationTrainingPipeline
 
 
 class LPTrainingPipeline(ClassificationTrainingPipeline[LPModel]):
+    """
+    Represents a link prediction training pipeline.
+    Construct an instance of this class using :func:`graphdatascience.GraphDataScience.lp_pipe`.
+    """
+
     def addFeature(self, feature_type: str, **config: Any) -> "Series[Any]":
+        """
+        Add a link feature to the pipeline.
+
+        Args:
+            feature_type: The type of feature to add.
+            **config: The configuration for the feature, this includes the node properties to use.
+
+        Returns:
+            The result of the query.
+        """
         query = f"{self._query_prefix()}addFeature($pipeline_name, $feature_type, $config)"
         params = {
             "pipeline_name": self.name(),
             "feature_type": feature_type,
             "config": config,
         }
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
     def feature_steps(self) -> DataFrame:
+        """
+        Get the feature steps of the pipeline.
+
+        Returns:
+            A DataFrame containing the feature steps of the pipeline.
+
+        """
         pipeline_info = self._list_info()["pipelineInfo"][0]
         return DataFrame(pipeline_info["featurePipeline"]["featureSteps"])
 
     def _query_prefix(self) -> str:
         return "CALL gds.beta.pipeline.linkPrediction."
 
     def _create_trained_model(self, name: str, query_runner: QueryRunner) -> LPModel:
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/nc_pipeline_create_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nc_pipeline_create_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from .nc_training_pipeline import NCTrainingPipeline
 
 
-class NCPipelineCreateRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class NCPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
     def create(self, name: str) -> Tuple[NCTrainingPipeline, "Series[Any]"]:
         self._namespace += ".create"
 
         query = f"CALL {self._namespace}($name)"
         params = {"name": name}
         result = self._query_runner.run_query(query, params).squeeze()
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/nc_training_pipeline.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nc_training_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,21 +5,43 @@
 
 from ..model.node_classification_model import NCModel
 from ..pipeline.classification_training_pipeline import ClassificationTrainingPipeline
 from ..query_runner.query_runner import QueryRunner
 
 
 class NCTrainingPipeline(ClassificationTrainingPipeline[NCModel], ABC):
+    """
+    Represents a node classification training pipeline.
+    Construct an instance of this class using :func:`graphdatascience.GraphDataScience.nc_pipe`.
+    """
+
     def selectFeatures(self, node_properties: Union[str, List[str]]) -> "Series[Any]":
+        """
+        Select the node properties to use for training.
+
+        Args:
+            node_properties: The node properties to use for training.
+
+        Returns:
+            The result of the query.
+
+        """
         query = f"{self._query_prefix()}selectFeatures($pipeline_name, $node_properties)"
         params = {"pipeline_name": self.name(), "node_properties": node_properties}
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
 
     def feature_properties(self) -> "Series[Any]":
+        """
+        Get the feature properties of the pipeline.
+
+        Returns:
+            A Series containing the feature properties of the pipeline.
+
+        """
         pipeline_info = self._list_info()["pipelineInfo"][0]
         feature_properties: "Series[Any]" = Series(pipeline_info["featurePipeline"]["featureProperties"], dtype=object)
         return feature_properties
 
     def _query_prefix(self) -> str:
         return "CALL gds.beta.pipeline.nodeClassification."
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/nr_pipeline_create_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/nr_pipeline_create_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from .nr_training_pipeline import NRTrainingPipeline
 
 
-class NRPipelineCreateRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class NRPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
     def create(self, name: str) -> Tuple[NRTrainingPipeline, "Series[Any]"]:
         self._namespace += ".create"
 
         query = f"CALL {self._namespace}($name)"
         params = {"name": name}
         result = self._query_runner.run_query(query, params).squeeze()
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/pipeline/pipeline_proc_runner.py` & `graphdatascience-1.7a1/graphdatascience/pipeline/pipeline_beta_proc_runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 from typing import Any, Optional
 
 from pandas import DataFrame, Series
 
-from ..caller_base import CallerBase
-from ..error.client_only_endpoint import client_only_endpoint
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from ..model.pipeline_model import PipelineModel
 from .lp_pipeline_create_runner import LPPipelineCreateRunner
-from .lp_training_pipeline import LPTrainingPipeline
 from .nc_pipeline_create_runner import NCPipelineCreateRunner
-from .nc_training_pipeline import NCTrainingPipeline
-from .nr_pipeline_create_runner import NRPipelineCreateRunner
-from .nr_training_pipeline import NRTrainingPipeline
 from .training_pipeline import TrainingPipeline
 
 
-class PipelineProcRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class PipelineBetaProcRunner(UncallableNamespace, IllegalAttrChecker):
     @property
     def linkPrediction(self) -> LPPipelineCreateRunner:
         return LPPipelineCreateRunner(self._query_runner, f"{self._namespace}.linkPrediction", self._server_version)
 
     @property
     def nodeClassification(self) -> NCPipelineCreateRunner:
         return NCPipelineCreateRunner(self._query_runner, f"{self._namespace}.nodeClassification", self._server_version)
 
-    @property
-    def nodeRegression(self) -> NRPipelineCreateRunner:
-        return NRPipelineCreateRunner(self._query_runner, f"{self._namespace}.nodeRegression", self._server_version)
-
     def list(self, pipeline: Optional[TrainingPipeline[PipelineModel]] = None) -> DataFrame:
         self._namespace += ".list"
 
         if pipeline:
             query = f"CALL {self._namespace}($pipeline_name)"
             params = {"pipeline_name": pipeline.name()}
         else:
@@ -52,29 +42,7 @@
     def drop(self, pipeline: TrainingPipeline[PipelineModel]) -> "Series[Any]":
         self._namespace += ".drop"
 
         query = f"CALL {self._namespace}($pipeline_name)"
         params = {"pipeline_name": pipeline.name()}
 
         return self._query_runner.run_query(query, params).squeeze()  # type: ignore
-
-    @client_only_endpoint("gds.pipeline")
-    def get(self, pipeline_name: str) -> TrainingPipeline[PipelineModel]:
-        query = "CALL gds.beta.pipeline.list($pipeline_name)"
-        params = {"pipeline_name": pipeline_name}
-        result = self._query_runner.run_query(query, params)
-
-        if len(result) == 0:
-            raise ValueError(f"No pipeline named '{pipeline_name}' exists")
-
-        pipeline_type = result["pipelineType"][0]
-        return self._resolve_pipeline(pipeline_type, pipeline_name)
-
-    def _resolve_pipeline(self, pipeline_type: str, pipeline_name: str) -> TrainingPipeline[PipelineModel]:
-        if pipeline_type == "Node classification training pipeline":
-            return NCTrainingPipeline(pipeline_name, self._query_runner, self._server_version)
-        elif pipeline_type == "Link prediction training pipeline":
-            return LPTrainingPipeline(pipeline_name, self._query_runner, self._server_version)
-        elif pipeline_type == "Node regression training pipeline":
-            return NRTrainingPipeline(pipeline_name, self._query_runner, self._server_version)
-
-        raise ValueError(f"Unknown model type encountered: '{pipeline_type}'")
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/query_runner/arrow_graph_constructor.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/arrow_graph_constructor.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,19 @@
             partitioned_dfs += numpy.array_split(df, num_batches)  # type: ignore
 
         return partitioned_dfs
 
     def _send_action(self, action_type: str, meta_data: Dict[str, Any]) -> None:
         result = self._client.do_action(flight.Action(action_type, json.dumps(meta_data).encode("utf-8")))
 
-        json.loads(next(result).body.to_pybytes().decode())
+        # Consume result fully to sanity check and avoid cancelled streams
+        collected_result = list(result)
+        assert len(collected_result) == 1
+
+        json.loads(collected_result[0].body.to_pybytes().decode())
 
     def _send_df(self, df: DataFrame, entity_type: str, pbar: tqdm) -> None:
         table = Table.from_pandas(df)
         batches = table.to_batches(self._chunk_size)
         flight_descriptor = {"name": self._graph_name, "entity_type": entity_type}
 
         # Write schema
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/query_runner/arrow_query_runner.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/arrow_query_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import time
 from typing import Any, Dict, List, Optional, Tuple
 
 import pyarrow.flight as flight
 from pandas import DataFrame
 from pyarrow.flight import ClientMiddleware, ClientMiddlewareFactory
 
+from ..server_version.server_version import ServerVersion
 from .arrow_graph_constructor import ArrowGraphConstructor
 from .graph_constructor import GraphConstructor
 from .query_runner import QueryRunner
 from graphdatascience.server_version.compatible_with import (
     IncompatibleServerVersionError,
 )
-from graphdatascience.server_version.server_version import ServerVersion
 
 
 class ArrowQueryRunner(QueryRunner):
     def __init__(
         self,
         uri: str,
         fallback_query_runner: QueryRunner,
@@ -43,15 +43,19 @@
             client_options["middleware"] = [AuthFactory(auth)]
         if tls_root_certs:
             client_options["tls_root_certs"] = tls_root_certs
 
         self._flight_client = flight.FlightClient(location, **client_options)
 
     def run_query(
-        self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
+        self,
+        query: str,
+        params: Optional[Dict[str, Any]] = None,
+        database: Optional[str] = None,
+        custom_error: bool = True,
     ) -> DataFrame:
         if params is None:
             params = {}
 
         new_endpoint_server_version = ServerVersion(2, 2, 0)
 
         # We need to support the deprecated endpoints until they get removed on the server side
@@ -122,15 +126,15 @@
                     f"server version >= 2.2.0. The current version is {self._server_version}"
                 )
             else:
                 endpoint = "gds.beta.graph.relationships.stream"
 
             return self._run_arrow_property_get(graph_name, endpoint, {"relationship_types": relationship_types})
 
-        return self._fallback_query_runner.run_query(query, params, database)
+        return self._fallback_query_runner.run_query(query, params, database, custom_error)
 
     def run_query_with_logging(
         self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
     ) -> DataFrame:
         # For now there's no logging support with Arrow queries.
         return self._fallback_query_runner.run_query_with_logging(query, params, database)
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/query_runner/cypher_graph_constructor.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/cypher_graph_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             rel_df = relationship_dfs[0]
 
             self.CyperProjectionRunner(self._query_runner, self._graph_name, self._concurrency).run(node_df, rel_df)
 
     def _should_warn_about_arrow_missing(self) -> bool:
         try:
             license: str = self._query_runner.run_query(
-                "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value"
+                "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value", custom_error=False
             ).squeeze()
             should_warn = license == "Licensed"
         except Exception as e:
             # It's not a user's concern whether Arrow is set up or not in AuraDS.
             if (
                 "There is no procedure with the name `gds.debug.sysInfo` "
                 "registered for this database instance." in str(e)
@@ -108,15 +108,14 @@
                 should_warn = False
             else:
                 raise e
 
         return should_warn
 
     class CypherAggregationRunner:
-
         _BIT_COL_SUFFIX = "_is_present" + str(uuid4())
 
         def __init__(
             self,
             query_runner: QueryRunner,
             graph_name: str,
             concurrency: int,
@@ -189,14 +188,15 @@
             self._query_runner.run_query(
                 query,
                 {
                     "data": combined_df.values.tolist(),
                     "graph_name": self._graph_name,
                     "configuration": configuration,
                 },
+                custom_error=False,
             )
 
         def check_value_clause(self, combined_cols: List[str], col: str) -> str:
             return (
                 f"CASE"
                 f" WHEN data[{combined_cols.index(col + self._BIT_COL_SUFFIX)}]"
                 f" THEN data[{combined_cols.index(col)}]"
@@ -343,14 +343,15 @@
                     "graph_name": self._graph_name,
                     "node_query": node_query,
                     "relationship_query": relationship_query,
                     "read_concurrency": self._concurrency,
                     "nodes": nodes,
                     "relationships": relationships,
                 },
+                custom_error=False,
             )
 
         def _node_query(self, node_df: DataFrame) -> Tuple[str, List[List[Any]]]:
             node_list = node_df.values.tolist()
             node_columns = list(node_df.columns)
             node_id_index = node_columns.index("nodeId")
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/query_runner/query_runner.py` & `graphdatascience-1.7a1/graphdatascience/query_runner/query_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 from ..server_version.server_version import ServerVersion
 from .graph_constructor import GraphConstructor
 
 
 class QueryRunner(ABC):
     @abstractmethod
     def run_query(
-        self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
+        self,
+        query: str,
+        params: Optional[Dict[str, Any]] = None,
+        database: Optional[str] = None,
+        custom_error: bool = True,
     ) -> DataFrame:
         pass
 
     def run_query_with_logging(
         self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
     ) -> DataFrame:
-        return self.run_query(query, params, database)
+        return self.run_query(query, params, database, True)
 
     @abstractmethod
     def set_database(self, database: str) -> None:
         pass
 
     def close(self) -> None:
         pass
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/cora/cora_nodes_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/cora/cora_nodes_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/cora/cora_rels_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/cora/cora_rels_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/cora/serialize_cora.py` & `graphdatascience-1.7a1/graphdatascience/resources/cora/serialize_cora.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_acted_in_rels_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_actors_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_actors_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directed_in_rels_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_directors_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_directors_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_with_genre_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/imdb_movies_without_genre_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/edges.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/edges.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/labels.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/labels.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/raw/node_features.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/raw/node_features.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/imdb/serialize_imdb.py` & `graphdatascience-1.7a1/graphdatascience/resources/imdb/serialize_imdb.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/resources/karate/karate_club_gzip.pkl` & `graphdatascience-1.7a1/graphdatascience/resources/karate/karate_club_gzip.pkl`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/server_version/compatible_with.py` & `graphdatascience-1.7a1/graphdatascience/server_version/compatible_with.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.6rc1/graphdatascience/server_version/server_version.py` & `graphdatascience-1.7a1/graphdatascience/server_version/server_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 
 class InvalidServerVersionError(Exception):
     pass
 
 
 class ServerVersion:
+    """
+    A representation of the version of the Neo4j Graph Data Science library installed on the server.
+    """
+
     def __init__(self, major: int, minor: int, patch: int):
         self.major = major
         self.minor = minor
         self.patch = patch
 
     @classmethod
     def from_string(cls: Type[SV], version: str) -> SV:
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/system/config_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/system/config_endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pandas import DataFrame
 
 from graphdatascience.caller_base import CallerBase
 from graphdatascience.error.illegal_attr_checker import IllegalAttrChecker
 from graphdatascience.error.uncallable_namespace import UncallableNamespace
 
 
-class ConfigProcRunner(CallerBase, IllegalAttrChecker, UncallableNamespace):
+class ConfigProcRunner(IllegalAttrChecker, UncallableNamespace):
     def set(self, key: str, value: Any, username: Optional[str] = None) -> None:
         self._namespace += ".set"
 
         params = {"key": key, "value": value}
 
         # Checking for explicit None as '' is a valid user
         if username is not None:
@@ -35,15 +35,21 @@
 
         query = f"CALL {self._namespace}($config)"
         params = {"config": config}
 
         return self._query_runner.run_query(query, params)
 
 
-class IndirectConfigEndpoints(CallerBase):
+class ConfigIntermediateSteps(CallerBase):
     @property
     def defaults(self) -> ConfigProcRunner:
         return ConfigProcRunner(self._query_runner, f"{self._namespace}.defaults", self._server_version)
 
     @property
     def limits(self) -> ConfigProcRunner:
         return ConfigProcRunner(self._query_runner, f"{self._namespace}.limits", self._server_version)
+
+
+class ConfigEndpoints(CallerBase):
+    @property
+    def config(self) -> ConfigIntermediateSteps:
+        return ConfigIntermediateSteps(self._query_runner, f"{self._namespace}.config", self._server_version)
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/system/system_endpoints.py` & `graphdatascience-1.7a1/graphdatascience/system/system_endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 from ..caller_base import CallerBase
 from ..error.client_only_endpoint import client_only_endpoint
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 
 
-class DebugProcRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class DebugProcRunner(UncallableNamespace, IllegalAttrChecker):
     def sysInfo(self) -> "Series[Any]":
         self._namespace += ".sysInfo"
         query = f"CALL {self._namespace}()"
 
         return self._query_runner.run_query(query).squeeze()  # type: ignore
 
 
 class DirectSystemEndpoints(CallerBase):
     @client_only_endpoint("gds")
     def is_licensed(self) -> bool:
         try:
             license: str = self._query_runner.run_query(
-                "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value"
+                "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value", custom_error=False
             ).squeeze()
         except Exception as e:
             # AuraDS does not have `gds.debug.sysInfo`, but is always GDS EE.
             if (
                 "There is no procedure with the name `gds.debug.sysInfo` "
                 "registered for this database instance." in str(e)
             ):
@@ -36,27 +36,29 @@
         return license == "Licensed"
 
     @property
     def debug(self) -> DebugProcRunner:
         return DebugProcRunner(self._query_runner, f"{self._namespace}.debug", self._server_version)
 
 
-class IndirectSystemEndpoints(CallerBase):
+class SystemBetaEndpoints(CallerBase):
     def listProgress(self, job_id: Optional[str] = None) -> DataFrame:
         self._namespace += ".listProgress"
 
         if job_id:
             query = f"CALL {self._namespace}($job_id)"
             params = {"job_id": job_id}
         else:
             query = f"CALL {self._namespace}()"
             params = {}
 
         return self._query_runner.run_query(query, params)
 
+
+class SystemAlphaEndpoints(CallerBase):
     def userLog(self) -> DataFrame:
         self._namespace += ".userLog"
         query = f"CALL {self._namespace}()"
 
         return self._query_runner.run_query(query)
 
     def systemMonitor(self) -> "Series[Any]":
```

### Comparing `graphdatascience-1.6rc1/graphdatascience/topological_lp/topological_lp_runner.py` & `graphdatascience-1.7a1/graphdatascience/topological_lp/topological_lp_alpha_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Dict, Optional
 
-from ..caller_base import CallerBase
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 
 
-class TopologicalLPRunner(CallerBase, UncallableNamespace, IllegalAttrChecker):
+class TopologicalLPAlphaRunner(UncallableNamespace, IllegalAttrChecker):
     def _run_standard_function(self, node1: int, node2: int, config: Dict[str, Any]) -> float:
         query = f"""
         MATCH (n1) WHERE id(n1) = {node1}
         MATCH (n2) WHERE id(n2) = {node2}
         RETURN {self._namespace}(n1, n2, $config) AS score
         """
         params = {"config": config}
```

### Comparing `graphdatascience-1.6rc1/graphdatascience.egg-info/PKG-INFO` & `graphdatascience-1.7a1/graphdatascience.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdatascience
-Version: 1.6rc1
+Version: 1.7a1
 Summary: A Python client for the Neo4j Graph Data Science (GDS) library
 Home-page: https://neo4j.com/product/graph-data-science/
 Author: Neo4j
 Author-email: team-gds@neo4j.org
 License: Apache License 2.0
 Project-URL: Documentation, https://neo4j.com/docs/graph-data-science-client/current/
 Project-URL: Source, https://github.com/neo4j/graph-data-science-client
@@ -16,20 +16,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: ogb
+Provides-Extra: networkx
 License-File: LICENSE
 
 # Neo4j Graph Data Science Client
 
 [![Latest version](https://img.shields.io/pypi/v/graphdatascience)](https://pypi.org/project/graphdatascience/)
 [![PyPI downloads month](https://img.shields.io/pypi/dm/graphdatascience)](https://pypi.org/project/graphdatascience/)
 ![Python versions](https://img.shields.io/pypi/pyversions/graphdatascience)
@@ -105,17 +108,17 @@
 
 The example here assumes using an AuraDS instance.
 For additional examples and extensive documentation of all capabilities, please refer to the [GDS Python Client Manual](https://neo4j.com/docs/graph-data-science-client/current/).
 
 Full end-to-end examples in Jupyter ready-to-run notebooks can be found in the [`examples` source directory](https://github.com/neo4j/graph-data-science-client/tree/main/examples):
 
 * [Machine learning pipelines: Node classification](examples/ml-pipelines-node-classification.ipynb)
-* [Node regression with subgraph and sampling projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
+* [Node Regression with Subgraph and Graph Sample projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
 * [Product recommendations with kNN based on FastRP embeddings](examples/fastrp-and-knn.ipynb)
-* [Exporting from GDS and running GNN with PyG](examples/import-sample-export-gnn.ipynb)
+* [Sampling, Export and Integration with PyG example](examples/import-sample-export-gnn.ipynb)
 * [Load data to a projected graph via graph construction](examples/load-data-via-graph-construction.ipynb)
 * [Heterogeneous Node Classification with HashGNN and Autotuning](https://github.com/neo4j/graph-data-science-client/tree/main/examples/heterogeneous-node-classification-with-hashgnn.ipynb)
 
 
 ## Documentation
 
 The primary source for learning everything about the GDS Python Client is the manual, hosted at https://neo4j.com/docs/graph-data-science-client/current/.
@@ -124,14 +127,15 @@
 
 ## Known limitations
 
 Operations known to not yet work with `graphdatascience`:
 
 * [Numeric utility functions](https://neo4j.com/docs/graph-data-science/current/management-ops/utility-functions/#utility-functions-numeric) (will never be supported)
 * [Cypher on GDS](https://neo4j.com/docs/graph-data-science/current/management-ops/create-cypher-db/) (might be supported in the future)
+* [Projecting graphs using Cypher Aggregation](https://neo4j.com/docs/graph-data-science/current/management-ops/projections/graph-project-cypher-aggregation/) (might be supported in the future)
 
 
 ## License
 
 `graphdatascience` is licensed under the Apache Software License version 2.0.
 All content is copyright © Neo4j Sweden AB.
```

### Comparing `graphdatascience-1.6rc1/graphdatascience.egg-info/SOURCES.txt` & `graphdatascience-1.7a1/graphdatascience.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,66 +2,79 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 graphdatascience/__init__.py
 graphdatascience/call_builder.py
 graphdatascience/caller_base.py
-graphdatascience/direct_endpoints.py
+graphdatascience/endpoints.py
 graphdatascience/graph_data_science.py
-graphdatascience/indirect_endpoints.py
+graphdatascience/ignored_server_endpoints.py
 graphdatascience/py.typed
 graphdatascience/version.py
 graphdatascience.egg-info/PKG-INFO
 graphdatascience.egg-info/SOURCES.txt
 graphdatascience.egg-info/dependency_links.txt
 graphdatascience.egg-info/not-zip-safe
 graphdatascience.egg-info/requires.txt
 graphdatascience.egg-info/top_level.txt
 graphdatascience/algo/__init__.py
 graphdatascience/algo/algo_endpoints.py
 graphdatascience/algo/algo_proc_runner.py
 graphdatascience/algo/single_mode_algo_endpoints.py
 graphdatascience/error/__init__.py
 graphdatascience/error/client_only_endpoint.py
+graphdatascience/error/deprecation_warning.py
+graphdatascience/error/endpoint_suggester.py
 graphdatascience/error/illegal_attr_checker.py
 graphdatascience/error/unable_to_connect.py
 graphdatascience/error/uncallable_namespace.py
 graphdatascience/graph/__init__.py
+graphdatascience/graph/graph_alpha_proc_runner.py
+graphdatascience/graph/graph_alpha_project_runner.py
+graphdatascience/graph/graph_beta_proc_runner.py
 graphdatascience/graph/graph_endpoints.py
 graphdatascience/graph/graph_entity_ops_runner.py
 graphdatascience/graph/graph_export_runner.py
 graphdatascience/graph/graph_object.py
 graphdatascience/graph/graph_proc_runner.py
 graphdatascience/graph/graph_project_runner.py
 graphdatascience/graph/graph_sample_runner.py
 graphdatascience/graph/graph_type_check.py
+graphdatascience/graph/nx_loader.py
+graphdatascience/graph/ogb_loader.py
 graphdatascience/model/__init__.py
 graphdatascience/model/graphsage_model.py
 graphdatascience/model/link_prediction_model.py
 graphdatascience/model/model.py
+graphdatascience/model/model_alpha_proc_runner.py
+graphdatascience/model/model_beta_proc_runner.py
 graphdatascience/model/model_endpoints.py
 graphdatascience/model/model_proc_runner.py
+graphdatascience/model/model_resolver.py
 graphdatascience/model/node_classification_model.py
 graphdatascience/model/node_regression_model.py
 graphdatascience/model/pipeline_model.py
 graphdatascience/pipeline/__init__.py
 graphdatascience/pipeline/classification_training_pipeline.py
 graphdatascience/pipeline/lp_pipeline_create_runner.py
 graphdatascience/pipeline/lp_training_pipeline.py
 graphdatascience/pipeline/nc_pipeline_create_runner.py
 graphdatascience/pipeline/nc_training_pipeline.py
 graphdatascience/pipeline/nr_pipeline_create_runner.py
 graphdatascience/pipeline/nr_training_pipeline.py
+graphdatascience/pipeline/pipeline_alpha_proc_runner.py
+graphdatascience/pipeline/pipeline_beta_proc_runner.py
 graphdatascience/pipeline/pipeline_endpoints.py
 graphdatascience/pipeline/pipeline_proc_runner.py
 graphdatascience/pipeline/training_pipeline.py
 graphdatascience/query_runner/__init__.py
 graphdatascience/query_runner/arrow_graph_constructor.py
 graphdatascience/query_runner/arrow_query_runner.py
+graphdatascience/query_runner/aura_db_arrow_query_runner.py
 graphdatascience/query_runner/cypher_graph_constructor.py
 graphdatascience/query_runner/graph_constructor.py
 graphdatascience/query_runner/neo4j_query_runner.py
 graphdatascience/query_runner/query_runner.py
 graphdatascience/resources/__init__.py
 graphdatascience/resources/cora/__init__.py
 graphdatascience/resources/cora/cora_nodes_gzip.pkl
@@ -83,13 +96,15 @@
 graphdatascience/server_version/__init__.py
 graphdatascience/server_version/compatible_with.py
 graphdatascience/server_version/server_version.py
 graphdatascience/system/__init__.py
 graphdatascience/system/config_endpoints.py
 graphdatascience/system/system_endpoints.py
 graphdatascience/topological_lp/__init__.py
+graphdatascience/topological_lp/topological_lp_alpha_runner.py
 graphdatascience/topological_lp/topological_lp_endpoints.py
-graphdatascience/topological_lp/topological_lp_runner.py
 graphdatascience/utils/__init__.py
 graphdatascience/utils/util_endpoints.py
 graphdatascience/utils/util_proc_runner.py
-requirements/base.txt
+requirements/base/base.txt
+requirements/base/networkx.txt
+requirements/base/ogb.txt
```

### Comparing `graphdatascience-1.6rc1/setup.py` & `graphdatascience-1.7a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-with open("requirements/base.txt", "r", encoding="utf-8") as f:
+with open("requirements/base/base.txt", "r", encoding="utf-8") as f:
     reqs = f.read().splitlines()
 
+with open("requirements/base/ogb.txt", "r", encoding="utf-8") as f:
+    ogb_reqs = f.read().splitlines()
+
+with open("requirements/base/networkx.txt", "r", encoding="utf-8") as f:
+    nx_reqs = f.read().splitlines()
+
 with open("graphdatascience/version.py") as f:
     version = f.readline().strip().split()[-1][1:-1]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -17,14 +23,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Database",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 project_urls = {
@@ -46,8 +53,9 @@
     classifiers=classifiers,
     packages=setuptools.find_packages(),
     package_data={"graphdatascience": ["py.typed", "resources/**/*.pkl"]},
     project_urls=project_urls,
     python_requires=">=3.7",
     install_requires=reqs,
     zip_safe=False,
+    extras_require={"ogb": ogb_reqs, "networkx": nx_reqs},
 )
```

