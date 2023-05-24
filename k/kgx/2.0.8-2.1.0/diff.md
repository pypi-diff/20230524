# Comparing `tmp/kgx-2.0.8.tar.gz` & `tmp/kgx-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgx-2.0.8.tar", max compression
+gzip compressed data, was "kgx-2.1.0.tar", max compression
```

## Comparing `kgx-2.0.8.tar` & `kgx-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1526 2023-05-11 14:31:41.233589 kgx-2.0.8/LICENSE
--rw-r--r--   0        0        0     6473 2023-05-11 14:31:41.233589 kgx-2.0.8/README.md
--rw-r--r--   0        0        0       42 2023-05-11 14:32:01.485552 kgx-2.0.8/kgx/__init__.py
--rw-r--r--   0        0        0    16105 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/cli/__init__.py
--rw-r--r--   0        0        0    39539 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/cli/cli_utils.py
--rw-r--r--   0        0        0     3900 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/config.py
--rw-r--r--   0        0        0      731 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/config.yml
--rw-r--r--   0        0        0     1942 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/curie_lookup_service.py
--rw-r--r--   0        0        0     5094 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/error_detection.py
--rw-r--r--   0        0        0        0 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph/__init__.py
--rw-r--r--   0        0        0    10649 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph/base_graph.py
--rw-r--r--   0        0        0    13455 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph/nx_graph.py
--rw-r--r--   0        0        0     8498 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph_operations/__init__.py
--rw-r--r--   0        0        0    28863 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph_operations/clique_merge.py
--rw-r--r--   0        0        0     5776 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph_operations/graph_merge.py
--rw-r--r--   0        0        0    36314 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph_operations/meta_knowledge_graph.py
--rw-r--r--   0        0        0    30601 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/graph_operations/summarize_graph.py
--rw-r--r--   0        0        0        0 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/parsers/__init__.py
--rw-r--r--   0        0        0     2156 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/parsers/ntriples_parser.py
--rw-r--r--   0        0        0     6617 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/prefix_manager.py
--rw-r--r--   0        0        0      274 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/__init__.py
--rw-r--r--   0        0        0     1703 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/graph_sink.py
--rw-r--r--   0        0        0     2335 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/json_sink.py
--rw-r--r--   0        0        0     2242 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/jsonl_sink.py
--rw-r--r--   0        0        0     9073 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/neo_sink.py
--rw-r--r--   0        0        0     1356 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/null_sink.py
--rw-r--r--   0        0        0    20032 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/rdf_sink.py
--rw-r--r--   0        0        0     1436 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/sink.py
--rw-r--r--   0        0        0    10327 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/sql_sink.py
--rw-r--r--   0        0        0     8070 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/sink/tsv_sink.py
--rw-r--r--   0        0        0      395 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/__init__.py
--rw-r--r--   0        0        0     2526 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/graph_source.py
--rw-r--r--   0        0        0     2399 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/json_source.py
--rw-r--r--   0        0        0     1821 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/jsonl_source.py
--rw-r--r--   0        0        0    18963 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/neo_source.py
--rw-r--r--   0        0        0    11785 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/obograph_source.py
--rw-r--r--   0        0        0     7503 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/owl_source.py
--rw-r--r--   0        0        0    30464 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/rdf_source.py
--rw-r--r--   0        0        0    12162 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/source.py
--rw-r--r--   0        0        0     8221 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/sssom_source.py
--rw-r--r--   0        0        0     3665 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/trapi_source.py
--rw-r--r--   0        0        0     9150 2023-05-11 14:31:41.237589 kgx-2.0.8/kgx/source/tsv_source.py
--rw-r--r--   0        0        0    16660 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/transformer.py
--rw-r--r--   0        0        0        0 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/utils/__init__.py
--rw-r--r--   0        0        0     4575 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/utils/graph_utils.py
--rw-r--r--   0        0        0    18032 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/utils/infores.py
--rw-r--r--   0        0        0    32009 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/utils/kgx_utils.py
--rw-r--r--   0        0        0     8159 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/utils/rdf_utils.py
--rw-r--r--   0        0        0    28313 2023-05-11 14:31:41.241589 kgx-2.0.8/kgx/validator.py
--rw-r--r--   0        0        0     1592 2023-05-11 14:32:01.481552 kgx-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 kgx-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-05-24 01:33:10.856163 kgx-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6932 2023-05-24 01:33:10.856163 kgx-2.1.0/README.md
+-rw-r--r--   0        0        0       42 2023-05-24 01:33:26.920274 kgx-2.1.0/kgx/__init__.py
+-rw-r--r--   0        0        0    16105 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/cli/__init__.py
+-rw-r--r--   0        0        0    39539 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/cli/cli_utils.py
+-rw-r--r--   0        0        0     3900 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/config.py
+-rw-r--r--   0        0        0      731 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/config.yml
+-rw-r--r--   0        0        0     1942 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/curie_lookup_service.py
+-rw-r--r--   0        0        0     5094 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/error_detection.py
+-rw-r--r--   0        0        0        0 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph/__init__.py
+-rw-r--r--   0        0        0    10649 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph/base_graph.py
+-rw-r--r--   0        0        0    13455 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph/nx_graph.py
+-rw-r--r--   0        0        0     8498 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph_operations/__init__.py
+-rw-r--r--   0        0        0    28863 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph_operations/clique_merge.py
+-rw-r--r--   0        0        0     5776 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph_operations/graph_merge.py
+-rw-r--r--   0        0        0    36314 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph_operations/meta_knowledge_graph.py
+-rw-r--r--   0        0        0    30601 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/graph_operations/summarize_graph.py
+-rw-r--r--   0        0        0        0 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/parsers/__init__.py
+-rw-r--r--   0        0        0     2156 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/parsers/ntriples_parser.py
+-rw-r--r--   0        0        0     6617 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/prefix_manager.py
+-rw-r--r--   0        0        0      274 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/__init__.py
+-rw-r--r--   0        0        0     1703 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/graph_sink.py
+-rw-r--r--   0        0        0     2335 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/json_sink.py
+-rw-r--r--   0        0        0     2242 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/jsonl_sink.py
+-rw-r--r--   0        0        0     9073 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/neo_sink.py
+-rw-r--r--   0        0        0     1356 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/null_sink.py
+-rw-r--r--   0        0        0    20032 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/rdf_sink.py
+-rw-r--r--   0        0        0     1436 2023-05-24 01:33:10.856163 kgx-2.1.0/kgx/sink/sink.py
+-rw-r--r--   0        0        0    10327 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/sink/sql_sink.py
+-rw-r--r--   0        0        0     8070 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/sink/tsv_sink.py
+-rw-r--r--   0        0        0      395 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/graph_source.py
+-rw-r--r--   0        0        0     2399 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/json_source.py
+-rw-r--r--   0        0        0     1821 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/jsonl_source.py
+-rw-r--r--   0        0        0    18963 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/neo_source.py
+-rw-r--r--   0        0        0    11785 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/obograph_source.py
+-rw-r--r--   0        0        0     7503 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/owl_source.py
+-rw-r--r--   0        0        0    30464 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/rdf_source.py
+-rw-r--r--   0        0        0    12162 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/source.py
+-rw-r--r--   0        0        0     8221 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/sssom_source.py
+-rw-r--r--   0        0        0     3665 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/trapi_source.py
+-rw-r--r--   0        0        0     9150 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/source/tsv_source.py
+-rw-r--r--   0        0        0    16660 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/transformer.py
+-rw-r--r--   0        0        0        0 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/utils/__init__.py
+-rw-r--r--   0        0        0     4575 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/utils/graph_utils.py
+-rw-r--r--   0        0        0    18032 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/utils/infores.py
+-rw-r--r--   0        0        0    32009 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/utils/kgx_utils.py
+-rw-r--r--   0        0        0     8159 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/utils/rdf_utils.py
+-rw-r--r--   0        0        0    28313 2023-05-24 01:33:10.860164 kgx-2.1.0/kgx/validator.py
+-rw-r--r--   0        0        0     1628 2023-05-24 01:33:26.916274 kgx-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8892 1970-01-01 00:00:00.000000 kgx-2.1.0/PKG-INFO
```

### Comparing `kgx-2.0.8/LICENSE` & `kgx-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/README.md` & `kgx-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,35 @@
 
 Internal representation is a property graph, specifically a networkx MultiDiGraph.
 
 The structure of this graph is expected to conform to the Biolink Model standard, as specified in the [KGX format specification](specification/kgx-format.md).
 
 In addition to the main code-base, KGX also provides a series of [command line operations](https://kgx.readthedocs.io/en/latest/examples.html#using-kgx-cli).
 
+### Example usage
+Validate:
+```bash
+poetry run kgx validate -i tsv tests/resources/merge/test2_nodes.tsv tests/resources/merge/test2_edges.tsv
+```
+
+Merge:
+```bash
+poetry run kgx merge —merge-config tests/resources/test-merge.yaml 
+```
+
+Graph Summary:
+```bash
+poetry run kgx graph-summary -i tests/resources/graph_nodes.tsv  -o summary.txt
+```
+
+Transform:
+```bash
+poetry run kgx transform —transform-config tests/resources/test-transform-tsv-rdf.yaml
+```
+
 ### Error Detection and Reporting
 
 Non-redundant JSON-formatted structured error logging is now provided in KGX Transformer, Validator, GraphSummary and MetaKnowledgeGraph operations.  See the various unit tests for the general design pattern (using the Validator as an example here):
 
 ```python
 from kgx.validator import Validator
 from kgx.transformer import Transformer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kgx-2.0.8/kgx/cli/__init__.py` & `kgx-2.1.0/kgx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/cli/cli_utils.py` & `kgx-2.1.0/kgx/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/config.py` & `kgx-2.1.0/kgx/config.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/config.yml` & `kgx-2.1.0/kgx/config.yml`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/curie_lookup_service.py` & `kgx-2.1.0/kgx/curie_lookup_service.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/error_detection.py` & `kgx-2.1.0/kgx/error_detection.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph/base_graph.py` & `kgx-2.1.0/kgx/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph/nx_graph.py` & `kgx-2.1.0/kgx/graph/nx_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph_operations/__init__.py` & `kgx-2.1.0/kgx/graph_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph_operations/clique_merge.py` & `kgx-2.1.0/kgx/graph_operations/clique_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph_operations/graph_merge.py` & `kgx-2.1.0/kgx/graph_operations/graph_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph_operations/meta_knowledge_graph.py` & `kgx-2.1.0/kgx/graph_operations/meta_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/graph_operations/summarize_graph.py` & `kgx-2.1.0/kgx/graph_operations/summarize_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/parsers/ntriples_parser.py` & `kgx-2.1.0/kgx/parsers/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/prefix_manager.py` & `kgx-2.1.0/kgx/prefix_manager.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/graph_sink.py` & `kgx-2.1.0/kgx/sink/graph_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/json_sink.py` & `kgx-2.1.0/kgx/sink/json_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/jsonl_sink.py` & `kgx-2.1.0/kgx/sink/jsonl_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/neo_sink.py` & `kgx-2.1.0/kgx/sink/neo_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/null_sink.py` & `kgx-2.1.0/kgx/sink/null_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/rdf_sink.py` & `kgx-2.1.0/kgx/sink/rdf_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/sink.py` & `kgx-2.1.0/kgx/sink/sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/sql_sink.py` & `kgx-2.1.0/kgx/sink/sql_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/sink/tsv_sink.py` & `kgx-2.1.0/kgx/sink/tsv_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/graph_source.py` & `kgx-2.1.0/kgx/source/graph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/json_source.py` & `kgx-2.1.0/kgx/source/json_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/jsonl_source.py` & `kgx-2.1.0/kgx/source/jsonl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/neo_source.py` & `kgx-2.1.0/kgx/source/neo_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/obograph_source.py` & `kgx-2.1.0/kgx/source/obograph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/owl_source.py` & `kgx-2.1.0/kgx/source/owl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/rdf_source.py` & `kgx-2.1.0/kgx/source/rdf_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/source.py` & `kgx-2.1.0/kgx/source/source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/sssom_source.py` & `kgx-2.1.0/kgx/source/sssom_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/trapi_source.py` & `kgx-2.1.0/kgx/source/trapi_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/source/tsv_source.py` & `kgx-2.1.0/kgx/source/tsv_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/transformer.py` & `kgx-2.1.0/kgx/transformer.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/utils/graph_utils.py` & `kgx-2.1.0/kgx/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/utils/infores.py` & `kgx-2.1.0/kgx/utils/infores.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/utils/kgx_utils.py` & `kgx-2.1.0/kgx/utils/kgx_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/utils/rdf_utils.py` & `kgx-2.1.0/kgx/utils/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/kgx/validator.py` & `kgx-2.1.0/kgx/validator.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.8/pyproject.toml` & `kgx-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kgx"
-version = "2.0.8"
+version = "2.1.0"
 description = "A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model."
 authors = ["Deepak Unni <deepak.unni3@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>", "Sierra Moxon <smoxon@lbl.gov>"]
 
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -15,16 +15,16 @@
 
 packages = [
     { include = "kgx" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-linkml = "^1.4"
-linkml-runtime = "^1.4"
+linkml = "^1.5.0"
+linkml-runtime = "^1.5.0"
 Sphinx = "*"
 python-dateutil = "^2.8.1"
 prefixcommons = "^0.1.4"
 docutils = "^0.18.1"
 networkx = "^2.8"
 SPARQLWrapper = "^1.8.2"
 pandas = "^1.0.3"
@@ -36,28 +36,30 @@
 pyyaml = "*"
 prologterms = "^0.0.6"
 shexjsg = "*"
 terminaltables = "^3.1.0"
 stringcase = "^1.2.0"
 validators = "^0.20.0"
 cachetools = "^5.0.0"
-sphinx-rtd-theme = "*"
-sphinx-click = "*"
 ordered-set = "^4.0.2"
 docker = "^6.0.0"
 jsonlines = "^3.1.0"
 jsonstreams = "^0.6.0"
 ijson = "^3.1.3"
 deprecation = "^2.1.0"
 recommonmark = "*"
 tox = "^3.0"
-bmt = "^1.0.13"
+bmt = "^1.0.15"
 inflection = "^0.5.1"
 closurizer = "^0.1.7"
 
+[tool.poetry.dev-dependencies]
+sphinx-rtd-theme = "*"
+sphinx-click = "*"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [build-system]
```

### Comparing `kgx-2.0.8/PKG-INFO` & `kgx-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 Metadata-Version: 2.1
 Name: kgx
-Version: 2.0.8
+Version: 2.1.0
 Summary: A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model.
 License: BSD
 Author: Deepak Unni
 Author-email: deepak.unni3@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: Click
 Requires-Dist: SPARQLWrapper (>=1.8.2,<2.0.0)
 Requires-Dist: Sphinx
-Requires-Dist: bmt (>=1.0.13,<2.0.0)
+Requires-Dist: bmt (>=1.0.15,<2.0.0)
 Requires-Dist: cachetools (>=5.0.0,<6.0.0)
 Requires-Dist: closurizer (>=0.1.7,<0.2.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: docutils (>=0.18.1,<0.19.0)
 Requires-Dist: ijson (>=3.1.3,<4.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: jsonstreams (>=0.6.0,<0.7.0)
-Requires-Dist: linkml (>=1.4,<2.0)
-Requires-Dist: linkml-runtime (>=1.4,<2.0)
+Requires-Dist: linkml (>=1.5.0,<2.0.0)
+Requires-Dist: linkml-runtime (>=1.5.0,<2.0.0)
 Requires-Dist: mypy
 Requires-Dist: neo4j (>=4.4.10,<5.0.0)
 Requires-Dist: networkx (>=2.8,<3.0)
 Requires-Dist: ordered-set (>=4.0.2,<5.0.0)
 Requires-Dist: pandas (>=1.0.3,<2.0.0)
 Requires-Dist: prefixcommons (>=0.1.4,<0.2.0)
 Requires-Dist: prologterms (>=0.0.6,<0.0.7)
 Requires-Dist: pytest
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pyyaml
 Requires-Dist: rdflib (>=6.3.1,<7.0.0)
 Requires-Dist: recommonmark
 Requires-Dist: shexjsg
-Requires-Dist: sphinx-click
-Requires-Dist: sphinx-rtd-theme
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: terminaltables (>=3.1.0,<4.0.0)
 Requires-Dist: tox (>=3.0,<4.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Knowledge Graph Exchange
@@ -81,14 +78,35 @@
 
 Internal representation is a property graph, specifically a networkx MultiDiGraph.
 
 The structure of this graph is expected to conform to the Biolink Model standard, as specified in the [KGX format specification](specification/kgx-format.md).
 
 In addition to the main code-base, KGX also provides a series of [command line operations](https://kgx.readthedocs.io/en/latest/examples.html#using-kgx-cli).
 
+### Example usage
+Validate:
+```bash
+poetry run kgx validate -i tsv tests/resources/merge/test2_nodes.tsv tests/resources/merge/test2_edges.tsv
+```
+
+Merge:
+```bash
+poetry run kgx merge —merge-config tests/resources/test-merge.yaml 
+```
+
+Graph Summary:
+```bash
+poetry run kgx graph-summary -i tests/resources/graph_nodes.tsv  -o summary.txt
+```
+
+Transform:
+```bash
+poetry run kgx transform —transform-config tests/resources/test-transform-tsv-rdf.yaml
+```
+
 ### Error Detection and Reporting
 
 Non-redundant JSON-formatted structured error logging is now provided in KGX Transformer, Validator, GraphSummary and MetaKnowledgeGraph operations.  See the various unit tests for the general design pattern (using the Validator as an example here):
 
 ```python
 from kgx.validator import Validator
 from kgx.transformer import Transformer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

