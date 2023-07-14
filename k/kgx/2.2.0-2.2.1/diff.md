# Comparing `tmp/kgx-2.2.0.tar.gz` & `tmp/kgx-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgx-2.2.0.tar", max compression
+gzip compressed data, was "kgx-2.2.1.tar", max compression
```

## Comparing `kgx-2.2.0.tar` & `kgx-2.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1526 2023-06-30 23:47:59.351944 kgx-2.2.0/LICENSE
--rw-r--r--   0        0        0     6932 2023-06-30 23:47:59.351944 kgx-2.2.0/README.md
--rw-r--r--   0        0        0       42 2023-06-30 23:48:17.372029 kgx-2.2.0/kgx/__init__.py
--rw-r--r--   0        0        0    16105 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/cli/__init__.py
--rw-r--r--   0        0        0    39539 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/cli/cli_utils.py
--rw-r--r--   0        0        0     3900 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/config.py
--rw-r--r--   0        0        0      731 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/config.yml
--rw-r--r--   0        0        0     1942 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/curie_lookup_service.py
--rw-r--r--   0        0        0     5094 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/error_detection.py
--rw-r--r--   0        0        0        0 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph/__init__.py
--rw-r--r--   0        0        0    10649 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph/base_graph.py
--rw-r--r--   0        0        0    13455 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph/nx_graph.py
--rw-r--r--   0        0        0     8498 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph_operations/__init__.py
--rw-r--r--   0        0        0    28863 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph_operations/clique_merge.py
--rw-r--r--   0        0        0     5776 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph_operations/graph_merge.py
--rw-r--r--   0        0        0    36314 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph_operations/meta_knowledge_graph.py
--rw-r--r--   0        0        0    30601 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/graph_operations/summarize_graph.py
--rw-r--r--   0        0        0        0 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/parsers/__init__.py
--rw-r--r--   0        0        0     2156 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/parsers/ntriples_parser.py
--rw-r--r--   0        0        0     6617 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/prefix_manager.py
--rw-r--r--   0        0        0      274 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/__init__.py
--rw-r--r--   0        0        0     1703 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/graph_sink.py
--rw-r--r--   0        0        0     2335 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/json_sink.py
--rw-r--r--   0        0        0     2242 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/jsonl_sink.py
--rw-r--r--   0        0        0     9073 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/neo_sink.py
--rw-r--r--   0        0        0     1356 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/null_sink.py
--rw-r--r--   0        0        0    20032 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/rdf_sink.py
--rw-r--r--   0        0        0     1436 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/sink.py
--rw-r--r--   0        0        0    10281 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/sql_sink.py
--rw-r--r--   0        0        0     8070 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/sink/tsv_sink.py
--rw-r--r--   0        0        0      395 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/source/__init__.py
--rw-r--r--   0        0        0     2526 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/source/graph_source.py
--rw-r--r--   0        0        0     2399 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/source/json_source.py
--rw-r--r--   0        0        0     1821 2023-06-30 23:47:59.355944 kgx-2.2.0/kgx/source/jsonl_source.py
--rw-r--r--   0        0        0    18963 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/neo_source.py
--rw-r--r--   0        0        0    11785 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/obograph_source.py
--rw-r--r--   0        0        0     7503 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/owl_source.py
--rw-r--r--   0        0        0    30464 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/rdf_source.py
--rw-r--r--   0        0        0    12162 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/source.py
--rw-r--r--   0        0        0     8221 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/sssom_source.py
--rw-r--r--   0        0        0     3665 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/trapi_source.py
--rw-r--r--   0        0        0     9150 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/source/tsv_source.py
--rw-r--r--   0        0        0    16660 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/transformer.py
--rw-r--r--   0        0        0        0 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/utils/__init__.py
--rw-r--r--   0        0        0     4575 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/utils/graph_utils.py
--rw-r--r--   0        0        0    18032 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/utils/infores.py
--rw-r--r--   0        0        0    32009 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/utils/kgx_utils.py
--rw-r--r--   0        0        0     8159 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/utils/rdf_utils.py
--rw-r--r--   0        0        0    28313 2023-06-30 23:47:59.359944 kgx-2.2.0/kgx/validator.py
--rw-r--r--   0        0        0     1605 2023-06-30 23:48:17.368028 kgx-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 kgx-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-07-14 13:02:53.241250 kgx-2.2.1/LICENSE
+-rw-r--r--   0        0        0     6932 2023-07-14 13:02:53.241250 kgx-2.2.1/README.md
+-rw-r--r--   0        0        0       42 2023-07-14 13:03:12.393647 kgx-2.2.1/kgx/__init__.py
+-rw-r--r--   0        0        0    16105 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/cli/__init__.py
+-rw-r--r--   0        0        0    39539 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/cli/cli_utils.py
+-rw-r--r--   0        0        0     3900 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/config.py
+-rw-r--r--   0        0        0      731 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/config.yml
+-rw-r--r--   0        0        0     1942 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/curie_lookup_service.py
+-rw-r--r--   0        0        0     5094 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/error_detection.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph/__init__.py
+-rw-r--r--   0        0        0    10649 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph/base_graph.py
+-rw-r--r--   0        0        0    13455 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph/nx_graph.py
+-rw-r--r--   0        0        0     8498 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph_operations/__init__.py
+-rw-r--r--   0        0        0    28863 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph_operations/clique_merge.py
+-rw-r--r--   0        0        0     5776 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph_operations/graph_merge.py
+-rw-r--r--   0        0        0    36314 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph_operations/meta_knowledge_graph.py
+-rw-r--r--   0        0        0    30601 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/graph_operations/summarize_graph.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/parsers/__init__.py
+-rw-r--r--   0        0        0     2156 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/parsers/ntriples_parser.py
+-rw-r--r--   0        0        0     6617 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/prefix_manager.py
+-rw-r--r--   0        0        0      274 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/__init__.py
+-rw-r--r--   0        0        0     1703 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/graph_sink.py
+-rw-r--r--   0        0        0     2335 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/json_sink.py
+-rw-r--r--   0        0        0     2242 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/jsonl_sink.py
+-rw-r--r--   0        0        0     9073 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/neo_sink.py
+-rw-r--r--   0        0        0     1356 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/null_sink.py
+-rw-r--r--   0        0        0    20032 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/rdf_sink.py
+-rw-r--r--   0        0        0     1436 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/sink.py
+-rw-r--r--   0        0        0    10281 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/sql_sink.py
+-rw-r--r--   0        0        0     8070 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/sink/tsv_sink.py
+-rw-r--r--   0        0        0      395 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/__init__.py
+-rw-r--r--   0        0        0     2526 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/graph_source.py
+-rw-r--r--   0        0        0     2399 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/json_source.py
+-rw-r--r--   0        0        0     1821 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/jsonl_source.py
+-rw-r--r--   0        0        0    18963 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/neo_source.py
+-rw-r--r--   0        0        0    11785 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/obograph_source.py
+-rw-r--r--   0        0        0     7503 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/owl_source.py
+-rw-r--r--   0        0        0    30464 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/rdf_source.py
+-rw-r--r--   0        0        0    12162 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/source.py
+-rw-r--r--   0        0        0     8221 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/sssom_source.py
+-rw-r--r--   0        0        0     3665 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/trapi_source.py
+-rw-r--r--   0        0        0     9150 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/source/tsv_source.py
+-rw-r--r--   0        0        0    16660 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/utils/__init__.py
+-rw-r--r--   0        0        0     4575 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/utils/graph_utils.py
+-rw-r--r--   0        0        0    18032 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/utils/infores.py
+-rw-r--r--   0        0        0    32009 2023-07-14 13:02:53.245250 kgx-2.2.1/kgx/utils/kgx_utils.py
+-rw-r--r--   0        0        0     8159 2023-07-14 13:02:53.249250 kgx-2.2.1/kgx/utils/rdf_utils.py
+-rw-r--r--   0        0        0    28313 2023-07-14 13:02:53.249250 kgx-2.2.1/kgx/validator.py
+-rw-r--r--   0        0        0     1605 2023-07-14 13:03:12.393647 kgx-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8840 1970-01-01 00:00:00.000000 kgx-2.2.1/PKG-INFO
```

### Comparing `kgx-2.2.0/LICENSE` & `kgx-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/README.md` & `kgx-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/cli/__init__.py` & `kgx-2.2.1/kgx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/cli/cli_utils.py` & `kgx-2.2.1/kgx/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/config.py` & `kgx-2.2.1/kgx/config.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/config.yml` & `kgx-2.2.1/kgx/config.yml`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/curie_lookup_service.py` & `kgx-2.2.1/kgx/curie_lookup_service.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/error_detection.py` & `kgx-2.2.1/kgx/error_detection.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph/base_graph.py` & `kgx-2.2.1/kgx/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph/nx_graph.py` & `kgx-2.2.1/kgx/graph/nx_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph_operations/__init__.py` & `kgx-2.2.1/kgx/graph_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph_operations/clique_merge.py` & `kgx-2.2.1/kgx/graph_operations/clique_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph_operations/graph_merge.py` & `kgx-2.2.1/kgx/graph_operations/graph_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph_operations/meta_knowledge_graph.py` & `kgx-2.2.1/kgx/graph_operations/meta_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/graph_operations/summarize_graph.py` & `kgx-2.2.1/kgx/graph_operations/summarize_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/parsers/ntriples_parser.py` & `kgx-2.2.1/kgx/parsers/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/prefix_manager.py` & `kgx-2.2.1/kgx/prefix_manager.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/graph_sink.py` & `kgx-2.2.1/kgx/sink/graph_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/json_sink.py` & `kgx-2.2.1/kgx/sink/json_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/jsonl_sink.py` & `kgx-2.2.1/kgx/sink/jsonl_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/neo_sink.py` & `kgx-2.2.1/kgx/sink/neo_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/null_sink.py` & `kgx-2.2.1/kgx/sink/null_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/rdf_sink.py` & `kgx-2.2.1/kgx/sink/rdf_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/sink.py` & `kgx-2.2.1/kgx/sink/sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/sql_sink.py` & `kgx-2.2.1/kgx/sink/sql_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/sink/tsv_sink.py` & `kgx-2.2.1/kgx/sink/tsv_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/graph_source.py` & `kgx-2.2.1/kgx/source/graph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/json_source.py` & `kgx-2.2.1/kgx/source/json_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/jsonl_source.py` & `kgx-2.2.1/kgx/source/jsonl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/neo_source.py` & `kgx-2.2.1/kgx/source/neo_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/obograph_source.py` & `kgx-2.2.1/kgx/source/obograph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/owl_source.py` & `kgx-2.2.1/kgx/source/owl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/rdf_source.py` & `kgx-2.2.1/kgx/source/rdf_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/source.py` & `kgx-2.2.1/kgx/source/source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/sssom_source.py` & `kgx-2.2.1/kgx/source/sssom_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/trapi_source.py` & `kgx-2.2.1/kgx/source/trapi_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/source/tsv_source.py` & `kgx-2.2.1/kgx/source/tsv_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/transformer.py` & `kgx-2.2.1/kgx/transformer.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/utils/graph_utils.py` & `kgx-2.2.1/kgx/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/utils/infores.py` & `kgx-2.2.1/kgx/utils/infores.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/utils/kgx_utils.py` & `kgx-2.2.1/kgx/utils/kgx_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/utils/rdf_utils.py` & `kgx-2.2.1/kgx/utils/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/kgx/validator.py` & `kgx-2.2.1/kgx/validator.py`

 * *Files identical despite different names*

### Comparing `kgx-2.2.0/pyproject.toml` & `kgx-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kgx"
-version = "2.2.0"
+version = "2.2.1"
 description = "A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model."
 authors = ["Deepak Unni <deepak.unni3@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>", "Sierra Moxon <smoxon@lbl.gov>"]
 
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -23,15 +23,15 @@
 linkml-runtime = "^1.5.0"
 Sphinx = "*"
 python-dateutil = "^2.8.1"
 prefixcommons = "^0.1.4"
 docutils = "^0.18.1"
 networkx = "^2.8"
 SPARQLWrapper = "^1.8.2"
-pandas = "^1.0.3"
+pandas = ">1.0.3"
 pytest = "*"
 mypy = "*"
 rdflib = "^6.3.1"
 Click = "*"
 neo4j = "^4.4.10"
 pyyaml = "*"
 prologterms = "^0.0.6"
```

### Comparing `kgx-2.2.0/PKG-INFO` & `kgx-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgx
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model.
 License: BSD
 Author: Deepak Unni
 Author-email: deepak.unni3@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -28,15 +28,15 @@
 Requires-Dist: jsonstreams (>=0.6.0,<0.7.0)
 Requires-Dist: linkml (>=1.5.0,<2.0.0)
 Requires-Dist: linkml-runtime (>=1.5.0,<2.0.0)
 Requires-Dist: mypy
 Requires-Dist: neo4j (>=4.4.10,<5.0.0)
 Requires-Dist: networkx (>=2.8,<3.0)
 Requires-Dist: ordered-set (>=4.0.2,<5.0.0)
-Requires-Dist: pandas (>=1.0.3,<2.0.0)
+Requires-Dist: pandas (>1.0.3)
 Requires-Dist: prefixcommons (>=0.1.4,<0.2.0)
 Requires-Dist: prologterms (>=0.0.6,<0.0.7)
 Requires-Dist: pytest
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pyyaml
 Requires-Dist: rdflib (>=6.3.1,<7.0.0)
 Requires-Dist: recommonmark
```

