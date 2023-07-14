# Comparing `tmp/langdash-1.7.4.tar.gz` & `tmp/langdash-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.7.4.tar", last modified: Mon Jul 10 01:52:12 2023, max compression
+gzip compressed data, was "langdash-1.7.5.tar", last modified: Fri Jul 14 03:46:15 2023, max compression
```

## Comparing `langdash-1.7.4.tar` & `langdash-1.7.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.642570 langdash-1.7.4/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.4/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.4/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-10 01:52:12.642570 langdash-1.7.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.7.4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-10 01:51:24.000000 langdash-1.7.4/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.4/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    15364 2023-07-10 01:47:58.000000 langdash-1.7.4/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.4/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.4/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.634570 langdash-1.7.4/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.4/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.4/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.4/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.4/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.4/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.4/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.642570 langdash-1.7.4/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.4/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.4/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.642570 langdash-1.7.4/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.4/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-07-09 01:44:13.000000 langdash-1.7.4/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.4/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.4/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.4/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.4/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.4/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.4/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    11281 2023-07-09 01:48:13.000000 langdash-1.7.4/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.4/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.4/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.4/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.634570 langdash-1.7.4/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.4/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.4/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.4/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.4/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-10 01:52:12.638570 langdash-1.7.4/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-10 01:52:12.000000 langdash-1.7.4/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-10 01:52:12.642570 langdash-1.7.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.403521 langdash-1.7.5/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.5/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.5/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-14 03:46:15.403521 langdash-1.7.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.7.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-14 03:45:48.000000 langdash-1.7.5/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.5/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15388 2023-07-11 02:58:29.000000 langdash-1.7.5/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.5/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.5/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.395520 langdash-1.7.5/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.5/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6868 2023-07-11 03:00:19.000000 langdash-1.7.5/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.7.5/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.5/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)      739 2023-07-11 02:58:29.000000 langdash-1.7.5/langdash/llm_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.5/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.5/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.5/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.5/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.403521 langdash-1.7.5/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.5/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-07-09 01:44:13.000000 langdash-1.7.5/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.5/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.5/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.5/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6112 2023-07-11 02:58:29.000000 langdash-1.7.5/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5810 2023-07-11 02:58:30.000000 langdash-1.7.5/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.5/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11977 2023-07-11 03:04:01.000000 langdash-1.7.5/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.5/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.5/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.5/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.395520 langdash-1.7.5/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.5/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.5/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.5/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.5/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 03:46:15.399520 langdash-1.7.5/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-14 03:46:15.000000 langdash-1.7.5/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-14 03:46:15.403521 langdash-1.7.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.5/setup.py
```

### Comparing `langdash-1.7.4/LICENSE.txt` & `langdash-1.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/PKG-INFO` & `langdash-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.4
+Version: 1.7.5
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.4/README.md` & `langdash-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/chains/chains.py` & `langdash-1.7.5/langdash/chains/chains.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,17 @@
     # argument/return checking
     for node in nodes:
       if isinstance(node, LDArg):
         if node._arg not in self._args:
           raise ValueError(f"'{node._arg}' not found in argument declaration")
       elif isinstance(node, (LDReturns, LDChoice)):
         if node._returns not in self._returns:
-          raise ValueError(f"'{node._returns}' not found in return declaration")
+          raise ValueError(
+            f"'{node._returns}' not found in return declaration"
+          )
 
     # fuse text nodes
     for i in range(len(pp_nodes)):
       pp_node_i = pp_nodes[i]
       if isinstance(pp_node_i, LDText):
         for j in range(i + 1, len(pp_nodes)):
           pp_node_j = pp_nodes[j]
```

### Comparing `langdash-1.7.4/langdash/chains/nodes.py` & `langdash-1.7.5/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/classify/token_qa.py` & `langdash-1.7.5/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/core.py` & `langdash-1.7.5/langdash/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,15 +214,18 @@
     """
     return chains.LDRepeat(self, *args, **kwargs)
 
   @staticmethod
   def model_from_type(type: str, *args, **kwargs) -> LLM:
     """
     Create an instance of a builtin model with specified type name.
-    Additional arguments will be passed to the model constructor.
+
+    Additional arguments will be passed to the model constructor. Alternatively,
+    a keyword argument with the name `config` of type `LLMConfig` can be passed
+    to specify config parameters.
     
     Args:
       type (str): The type of the model.
     
     Returns:
       The model.
     """
```

### Comparing `langdash-1.7.4/langdash/infer.py` & `langdash-1.7.5/langdash/infer.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,14 @@
   """ Maximum number of tokens to look back for repetition penalty. """
 
   rep_penalty: float = 1.0
   """ Repetition penalty, applied to logits for every repeated token before sampling. """
 
   def __post_init__(self):
     assert self.min_new_tokens >= 0
-    assert self.max_new_tokens >= 0
+    assert self.max_new_tokens >= self.min_new_tokens
     assert 0.0 <= self.temperature <= 10.0
     assert 0 <= self.top_k
     assert 0.0 <= self.top_p <= 1.0
     assert 0.0 <= self.typical_mass <= 1.0
     assert 0 <= self.max_rep_ctx
     assert 0.0 <= self.rep_penalty <= 10.0
```

### Comparing `langdash-1.7.4/langdash/llm.py` & `langdash-1.7.5/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/llm_session.py` & `langdash-1.7.5/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.7.5/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/_tokenizer/_bpe.py` & `langdash-1.7.5/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.7.5/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.7.5/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.7.5/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.7.5/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/ctransformers.py` & `langdash-1.7.5/langdash/models/llama_cpp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,104 @@
-from typing import List, Optional, Any
+from typing import List, Optional
 import weakref
 import torch
+from llama_cpp import Llama, LlamaState, llama_token_to_str  # type: ignore
 
 from langdash.llm import LLM
+from langdash.llm_config import LLMConfig
 from langdash.llm_session import LLMGenerationSessionForRawText
 import langdash.sampling as sampling
-from ._tokenizer.tokenizer import Tokenizer
 from ._tokenizer.bytes_dict_tokenizer import BytesDictTokenizer
-from ._tokenizer.hf_tokenizer import HFTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferWithSessionMixin
 
-import ctransformers  # type: ignore
-from ctransformers.llm import LLM as CTransformersLLM, LLMState as CTransformersState  # type: ignore
 
-
-class CTransformersWrapper:
-  model: CTransformersLLM
-  tokenizer: Tokenizer
-  vocab: List[bytes]
+class LlamaWrapper:
+  model: Llama
+  tokenizer: BytesDictTokenizer
   last_called_session: Optional[weakref.ref]
   eos_token: int
+  bos_token: int
 
-  def __init__(
-    self, model_path: str, tokenizer: Optional[Any] = None, *args, **kwargs
-  ):
-    self.model = ctransformers.AutoModelForCausalLM.from_pretrained(
-      model_path, **kwargs
+  def __init__(self, *args, **kwargs):
+    self.model = Llama(*args, **kwargs)
+    mapping = [
+      llama_token_to_str(self.model.ctx, tokid)
+      for tokid in range(self.model.n_vocab())
+    ]
+    self.tokenizer = BytesDictTokenizer(
+      lambda text, **_k: self.model.
+      tokenize(text.encode("utf-8"), add_bos=False),
+      lambda tokens, **_k: self.model.detokenize(tokens).decode("utf-8"),
+      mapping
     )
-    if tokenizer is not None:
-      self.tokenizer = HFTokenizer(tokenizer)
-    else:
-      mapping = [
-        self.model.token_id_to_str(tokid)
-        for tokid in range(self.model.vocab_size)
-      ]
-      self.tokenizer = BytesDictTokenizer(
-        lambda text, **_k: self.model.tokenize(text),
-        lambda tokens: self.model.detokenize(tokens), mapping
-      )
-    self.eos_token = self.model.eos_token_id
     self.last_called_session = None
+    self.eos_token = Llama.token_eos()
+    self.bos_token = Llama.token_bos()
 
   def eval(self, tokens: List[int]) -> torch.Tensor:
     self.model.eval(tokens)
-    return torch.tensor(self.model.logits)
+    return torch.from_numpy(self.model._scores[-1, :])
 
-  def enter_session(self, session: "CTransformersSession"):
+  def enter_session(self, session: "LlamaCppSession"):
     if self.last_called_session is None:
       self.last_called_session = weakref.ref(session)
       return
     last_called_session = self.last_called_session()
     if session == last_called_session:
       return
     elif last_called_session is not None:
-      last_called_session._logits = self.load_logits_from_model()
+      last_called_session._logits = self.load_logits_from_llama()
       last_called_session._state = self.model.save_state()
     if session._state is not None:
-      self.model.set_state(session._state)
+      self.model.load_state(session._state)
     self.last_called_session = weakref.ref(session)
 
-  def load_logits_from_model(self) -> torch.Tensor:
+  def load_logits_from_llama(self) -> torch.Tensor:
     return torch.Tensor(self.model.eval_logits[-1])
 
-  def clone_state(self, session: "CTransformersSession") -> CTransformersState:
+  def clone_state(self, session: "LlamaCppSession") -> LlamaState:
     self.enter_session(session)
-    return self.model.clone_state()
+    return self.model.save_state()
 
-  def set_state(
-    self, session: "CTransformersSession", state: Optional[CTransformersState]
-  ):
+  def set_state(self, session: "LlamaCppSession", state: Optional[LlamaState]):
     self.enter_session(session)
     self.model.reset()
     if state is not None:
-      self.model.set_state(state)
+      self.model.load_state(state)
 
   def get_context_length(self) -> int:
     # self.enter_session(self)
-    return self.model.context_length
+    return self.model.n_ctx()
 
 
-class CTransformersSession(
+class LlamaCppSession(
   TensorBasedInferWithSessionMixin,
-  LLMGenerationSessionForRawText["CTransformersModel", CTransformersState,
-                                 torch.Tensor]
+  LLMGenerationSessionForRawText["LlamaCppModel", LlamaState, torch.Tensor]
 ):
   """
-  Session for ctransformers model.
+  Session for llama.cpp model.
   """
 
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
-    def load_model(llm: CTransformersModel):
-      return CTransformersWrapper(
-        model_path=llm._model_path, **llm._model_kwargs
-      )
+    def load_model(llm: LlamaCppModel):
+      return LlamaWrapper(model_path=llm._model_path, **llm._model_kwargs)
 
     self._model = self._ld._get_model_internal(self._llm, load_model)
-
     self._logits = None
     self._state = None
     self._next_token = None
 
   def _eval(self, token: int):
     return self._model.eval([token])
 
   def _eval_mult(self, tokens: List[int]):
     return self._model.eval(tokens)
 
-  def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return self._model.tokenizer.encode(
-      text, add_special_tokens=add_special_tokens
-    )
-
-  def decode(self, tokids: List[int]) -> str:
-    return self._model.tokenizer.decode(tokids)
-
   def _next_token_logits_raw(self):
     self._model.enter_session(self)
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
@@ -128,44 +107,81 @@
 
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
-  def set_state(self, state: Optional[CTransformersState]):
+  def set_state(self, state: Optional[LlamaState]):
     self._model.set_state(self, state)
     if state is None:
       self._logits = None
     else:
-      self._logits = self._model.load_logits_from_model()
+      self._logits = self._model.load_logits_from_llama()
 
-  def clone_state(self) -> CTransformersState:
+  def clone_state(self) -> LlamaState:
     return self._model.clone_state(self)
 
+  def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
+    return self._model.tokenizer.encode(
+      text, add_special_tokens=add_special_tokens
+    )
+
+  def decode(self, tokens: List[int]) -> str:
+    return self._model.tokenizer.decode(tokens)
+
+  def _on_first_inject(self):
+    self._model.model.reset()
+    self._eval(self._model.bos_token)
+
   def get_context_length(self) -> int:
-    return self._model.get_context_length(self)
+    return self.model.get_context_length(self)
 
   # Wrapper for public functions to flush the old session states
 
   def inject(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
   def flush_token(self, *a, **k):
     self._model.enter_session(self)
     return LLMGenerationSessionForRawText.inject(self, *a, **k)
 
 
-class CTransformersModel(LLM[CTransformersSession]):
+class LlamaCppModel(LLM[LlamaCppSession]):
   """
   llama.cpp model.
   """
 
-  Session = CTransformersSession
+  _model_path: str
+  _model_kwargs: dict
+
+  Session = LlamaCppSession
+
+  def __init__(self, model_path: Optional[str] = None, **model_kwargs):
+    """
+    Creates a template for the Llama language model (using the llama.cpp library).
+    """
+    if "config" in model_kwargs:
+      if not isinstance(model_kwargs["config"], LLMConfig):
+        raise TypeError("config argument must be LLMConfig")
+
+      config = model_kwargs["config"]
+      del model_kwargs["config"]
+
+      self._model_kwargs = {
+        "n_batch": config.batch_size,
+        "n_threads": None if config.threads == -1 else config.threads,
+        "n_ctx": 512 if config.context_length == -1 else config.context_length,
+        "n_gpu_layers": config.gpu_layers,
+      }
+      self._model_kwargs.update(model_kwargs)
+      model_path = config.model
+    else:
+      self._model_kwargs = model_kwargs
 
-  def __init__(self, model_path: str, **model_kwargs):
+    if not isinstance(model_path, str):
+      raise TypeError("model path must be string")
     self._model_path = model_path
-    self._model_kwargs = model_kwargs
 
   def session(self, **kwargs):
-    return CTransformersSession(self, **kwargs)
+    return LlamaCppSession(self, **kwargs)
```

### Comparing `langdash-1.7.4/langdash/models/mock.py` & `langdash-1.7.5/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/rwkv_cpp.py` & `langdash-1.7.5/langdash/models/rwkv_cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import copy
 import os
 import sys
 import torch
 import tokenizers  # type: ignore
 
 from langdash.llm import LLM
+from langdash.llm_config import LLMConfig
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
@@ -162,15 +163,15 @@
   def __init__(self, llm: "RwkvCppModel"):
     assert _rwkv_lib is not None
     self.model = rwkv_cpp_model.RWKVModel(
       rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path,
       **llm._model_kwargs
     )
     self.batch_size = llm._batch_size
-    if self.batch_size == 1:
+    if self.batch_size <= 1:
       self.do_eval_sequence = False
     elif RWKV_CPP_ENABLE_EVAL_SEQUENCE:
       self.do_eval_sequence = hasattr(self.model, "eval_sequence")
     else:
       self.do_eval_sequence = False
     if llm._tokenizer_type == "20B":
       from ._tokenizer.rwkv_tokenizer import RwkvTokenizer
@@ -295,22 +296,28 @@
 
 
 class RwkvCppModel(LLM[RwkvCppSession]):
   """
   rwkv.cpp model
   """
 
+  _model_path: str
+  _model_kwargs: dict
+  _tokenizer_path: str
+  _tokenizer_type: str
+  _batch_size: int
+
   Session = RwkvCppSession
 
   def __init__(
     self,
-    model_path: str,
+    model_path: Optional[str] = None,
     tokenizer_path: Optional[str] = None,
     tokenizer_type: str = "20B",
-    batch_size: int = 32,
+    batch_size: int = 128,
     **model_kwargs
   ):
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
   
     You can pass the following environment variables to set compile flags:
   
@@ -330,31 +337,46 @@
         Path to the tokenizer file.
         Defaults to `None`. If not set, the built-in tokenizer will be used.
       tokenizer_type (str):
         The type of tokenizer to use. Either `"world"` for world models
         or `"20B"` for anything else.
       batch_size (int):
         The batch size for sequence evaluation.
-        Must be a positive integer (more than 0). If set to 1, serial evaluation
-        will always be used.
+        Must be a positive integer (more than 0).
+        If negative, serial evaluation will always be used.
     """
+    if "config" in model_kwargs:
+      if not isinstance(model_kwargs["config"], LLMConfig):
+        raise TypeError("config argument must be LLMConfig")
+
+      config = model_kwargs["config"]
+      del model_kwargs["config"]
+
+      self._model_kwargs = {
+        "thread_count": None if config.threads == -1 else config.threads,
+        "gpu_layer_count": config.gpu_layers,
+      }
+      self._model_kwargs.update(model_kwargs)
+      model_path = config.model
+      batch_size = config.batch_size
+    else:
+      self._model_kwargs = model_kwargs
+
+    if not isinstance(model_path, str):
+      raise TypeError("model path must be string")
+    self._model_path = model_path
+    self._batch_size = batch_size
 
     if not _rwkv_tokenizer_available and tokenizer_type != "20B":
       raise ValueError("old RWKV tokenizer only supports '20B'")
-    if batch_size < 1:
-      raise ValueError("batch_size must be >= 1")
-
-    self._model_path = model_path
     self._tokenizer_type = tokenizer_type
     if tokenizer_path is None:
       builtin_tokenizer_paths = {
         "world": "rwkv/rwkv_vocab_v20230424.txt",
         "20B": "rwkv/20B_tokenizer.json",
       }
       assert _rwkv_cpp_folder is not None
       self._tokenizer_path = os.path.join(
         _rwkv_cpp_folder, builtin_tokenizer_paths[self._tokenizer_type]
       )
     else:
       self._tokenizer_path = tokenizer_path
-    self._batch_size = batch_size
-    self._model_kwargs = model_kwargs
```

### Comparing `langdash-1.7.4/langdash/models/sentence_transformers.py` & `langdash-1.7.5/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/models/transformers.py` & `langdash-1.7.5/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/response.py` & `langdash-1.7.5/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/sampling.py` & `langdash-1.7.5/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/search/embedding_search.py` & `langdash-1.7.5/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/search/engine.py` & `langdash-1.7.5/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash/search/multichoice_search.py` & `langdash-1.7.5/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.4/langdash.egg-info/PKG-INFO` & `langdash-1.7.5/langdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.4
+Version: 1.7.5
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.4/langdash.egg-info/SOURCES.txt` & `langdash-1.7.5/langdash.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ./langdash/search/embedding_search.py
 ./langdash/search/engine.py
 ./langdash/search/multichoice_search.py
 langdash/__init__.py
 langdash/core.py
 langdash/infer.py
 langdash/llm.py
+langdash/llm_config.py
 langdash/llm_session.py
 langdash/response.py
 langdash/sampling.py
 langdash.egg-info/PKG-INFO
 langdash.egg-info/SOURCES.txt
 langdash.egg-info/dependency_links.txt
 langdash.egg-info/requires.txt
```

### Comparing `langdash-1.7.4/setup.py` & `langdash-1.7.5/setup.py`

 * *Files identical despite different names*

