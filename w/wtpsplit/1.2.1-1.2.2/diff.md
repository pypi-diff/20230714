# Comparing `tmp/wtpsplit-1.2.1.tar.gz` & `tmp/wtpsplit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-2pycv7yb/wtpsplit-1.2.1.tar", last modified: Tue Jul 11 18:17:13 2023, max compression
+gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-pbx5h2v6/wtpsplit-1.2.2.tar", last modified: Fri Jul 14 15:56:10 2023, max compression
```

## Comparing `wtpsplit-1.2.1.tar` & `wtpsplit-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/LICENSE
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    11432 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/README.md
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/pyproject.toml
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/setup.cfg
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-11 18:16:23.000000 wtpsplit-1.2.1/setup.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/wtpsplit/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14323 2023-07-11 18:13:22.000000 wtpsplit-1.2.1/wtpsplit/__init__.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/configs.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/wtpsplit/data/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/wtpsplit/data/language_info.csv
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/wtpsplit/data/punctuation.json
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.1/wtpsplit/data/punctuation.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5384 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/extract.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/models.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6374 2023-07-11 18:11:57.000000 wtpsplit-1.2.1/wtpsplit/utils.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-11 18:17:13.364403 wtpsplit-1.2.1/wtpsplit.egg-info/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/requires.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-11 18:17:13.000000 wtpsplit-1.2.1/wtpsplit.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/LICENSE
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    13141 2023-07-14 15:52:54.000000 wtpsplit-1.2.2/README.md
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-11 18:11:57.000000 wtpsplit-1.2.2/pyproject.toml
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/setup.cfg
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-14 15:52:01.000000 wtpsplit-1.2.2/setup.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.274079 wtpsplit-1.2.2/wtpsplit/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14632 2023-07-14 15:52:07.000000 wtpsplit-1.2.2/wtpsplit/__init__.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-11 18:11:57.000000 wtpsplit-1.2.2/wtpsplit/configs.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/wtpsplit/data/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/wtpsplit/data/language_info.csv
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/wtpsplit/data/punctuation.json
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/wtpsplit/data/punctuation.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5384 2023-07-11 18:11:57.000000 wtpsplit-1.2.2/wtpsplit/extract.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-13 18:24:26.000000 wtpsplit-1.2.2/wtpsplit/models.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6949 2023-07-14 15:48:34.000000 wtpsplit-1.2.2/wtpsplit/utils.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.274079 wtpsplit-1.2.2/wtpsplit.egg-info/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/requires.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/top_level.txt
```

### Comparing `wtpsplit-1.2.1/LICENSE` & `wtpsplit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.1/README.md` & `wtpsplit-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -252,21 +252,27 @@
 | zu  | Zulu                   |
 
 ## Citation
 
 Please cite `wtpsplit` as 
 
 ```
-@misc{minixhofer2023wheres,
-      title={Where's the Point? Self-Supervised Multilingual Punctuation-Agnostic Sentence Segmentation}, 
-      author={Benjamin Minixhofer and Jonas Pfeiffer and Ivan Vulić},
-      year={2023},
-      eprint={2305.18893},
-      archivePrefix={arXiv},
-      primaryClass={cs.CL}
+@inproceedings{minixhofer-etal-2023-wheres,
+    title = "Where{'}s the Point? Self-Supervised Multilingual Punctuation-Agnostic Sentence Segmentation",
+    author = "Minixhofer, Benjamin  and
+      Pfeiffer, Jonas  and
+      Vuli{\'c}, Ivan",
+    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
+    month = jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+    url = "https://aclanthology.org/2023.acl-long.398",
+    pages = "7215--7235",
+    abstract = "Many NLP pipelines split text into sentences as one of the crucial preprocessing steps. Prior sentence segmentation tools either rely on punctuation or require a considerable amount of sentence-segmented training data: both central assumptions might fail when porting sentence segmenters to diverse languages on a massive scale. In this work, we thus introduce a multilingual punctuation-agnostic sentence segmentation method, currently covering 85 languages, trained in a self-supervised fashion on unsegmented text, by making use of newline characters which implicitly perform segmentation into paragraphs. We further propose an approach that adapts our method to the segmentation in a given corpus by using only a small number (64-256) of sentence-segmented examples. The main results indicate that our method outperforms all the prior best sentence-segmentation tools by an average of 6.1{\%} F1 points. Furthermore, we demonstrate that proper sentence segmentation has a point: the use of a (powerful) sentence segmenter makes a considerable difference for a downstream application such as machine translation (MT). By using our method to match sentence segmentation to the segmentation used during training of MT models, we achieve an average improvement of 2.3 BLEU points over the best prior segmentation tool, as well as massive gains over a trivial segmenter that splits text into equally-sized blocks.",
 }
 ```
 
 ## Acknowledgments
 
 Ivan Vulić is supported by a personal Royal Society University Research Fellowship ‘Inclusive and Sustainable Language Technology for a Truly Multilingual World’ (no 221137; 2022–). Research supported with Cloud TPUs from Google’s TPU Research Cloud (TRC). We thank Christoph Minixhofer for advice in the initial stage of this project. We also thank Sebastian Ruder and Srini Narayanan for helpful feedback on a draft of the paper.
```

### Comparing `wtpsplit-1.2.1/setup.py` & `wtpsplit-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="wtpsplit",
-    version="1.2.1",
+    version="1.2.2",
     packages=["wtpsplit"],
     description="Robust, adaptible sentence segmentation for 85 languages",
     author="Benjamin Minixhofer",
     author_email="bminixhofer@gmail.com",
     install_requires=[
         "onnxruntime>=1.13.1",
         "transformers>=4.22.2",
```

### Comparing `wtpsplit-1.2.1/wtpsplit/__init__.py` & `wtpsplit-1.2.2/wtpsplit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import skops.io as sio
 from transformers import AutoConfig, AutoModelForTokenClassification
 from transformers.utils.hub import cached_file
 
 from wtpsplit.extract import ORTWrapper, PyTorchWrapper, extract
 from wtpsplit.utils import Constants, indices_to_sentences, sigmoid
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 
 class WtP:
     def __init__(
         self,
         model_name_or_model,
         from_pretrained_kwargs=None,
@@ -261,14 +261,15 @@
         stride=64,
         block_size: int = 512,
         batch_size=32,
         pad_last_batch: bool = False,
         remove_whitespace_before_inference: bool = False,
         outer_batch_size=1000,
         paragraph_threshold: float = 0.5,
+        strip_whitespace: bool = False,
         do_paragraph_segmentation=False,
         verbose: bool = False,
     ):
         if isinstance(text_or_texts, str):
             return next(
                 self._split(
                     [text_or_texts],
@@ -278,14 +279,15 @@
                     stride=stride,
                     block_size=block_size,
                     batch_size=batch_size,
                     pad_last_batch=pad_last_batch,
                     remove_whitespace_before_inference=remove_whitespace_before_inference,
                     outer_batch_size=outer_batch_size,
                     paragraph_threshold=paragraph_threshold,
+                    strip_whitespace=strip_whitespace,
                     do_paragraph_segmentation=do_paragraph_segmentation,
                     verbose=verbose,
                 )
             )
         else:
             return self._split(
                 text_or_texts,
@@ -295,14 +297,15 @@
                 stride=stride,
                 block_size=block_size,
                 batch_size=batch_size,
                 pad_last_batch=pad_last_batch,
                 remove_whitespace_before_inference=remove_whitespace_before_inference,
                 outer_batch_size=outer_batch_size,
                 paragraph_threshold=paragraph_threshold,
+                strip_whitespace=strip_whitespace,
                 do_paragraph_segmentation=do_paragraph_segmentation,
                 verbose=verbose,
             )
 
     def get_threshold(self, lang_code: str, style: str, return_punctuation_threshold: bool = False):
         try:
             _, _, punctuation_threshold, threshold = self.mixtures[lang_code][style]
@@ -324,14 +327,15 @@
         block_size: int,
         batch_size: int,
         pad_last_batch: bool,
         remove_whitespace_before_inference: bool,
         outer_batch_size: int,
         paragraph_threshold: float,
         do_paragraph_segmentation: bool,
+        strip_whitespace: bool,
         verbose: bool,
     ):
         if style is not None:
             if lang_code is None:
                 raise ValueError("Please specify a `lang_code` when passing a `style` to adapt to.")
 
             if self.mixtures is None:
@@ -368,23 +372,28 @@
             if do_paragraph_segmentation:
                 sentence_probs, newline_probs = probs
 
                 offset = 0
 
                 paragraphs = []
 
-                # TODO: indices_to_sentences should not be in evaluation module?
                 for paragraph in indices_to_sentences(text, np.where(newline_probs > paragraph_threshold)[0]):
                     sentences = []
 
                     for sentence in indices_to_sentences(
-                        paragraph, np.where(sentence_probs[offset : offset + len(paragraph)] > sentence_threshold)[0]
+                        paragraph,
+                        np.where(
+                            sentence_probs[offset : offset + len(paragraph)] > sentence_threshold,
+                        )[0],
+                        strip_whitespace=strip_whitespace,
                     ):
                         sentences.append(sentence)
 
                     paragraphs.append(sentences)
                     offset += len(paragraph)
 
                 yield paragraphs
             else:
-                sentences = indices_to_sentences(text, np.where(probs > sentence_threshold)[0])
+                sentences = indices_to_sentences(
+                    text, np.where(probs > sentence_threshold)[0], strip_whitespace=strip_whitespace
+                )
                 yield sentences
```

### Comparing `wtpsplit-1.2.1/wtpsplit/configs.py` & `wtpsplit-1.2.2/wtpsplit/configs.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.1/wtpsplit/data/language_info.csv` & `wtpsplit-1.2.2/wtpsplit/data/language_info.csv`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.1/wtpsplit/data/punctuation.json` & `wtpsplit-1.2.2/wtpsplit/data/punctuation.json`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.1/wtpsplit/extract.py` & `wtpsplit-1.2.2/wtpsplit/extract.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.1/wtpsplit/models.py` & `wtpsplit-1.2.2/wtpsplit/models.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.1/wtpsplit/utils.py` & `wtpsplit-1.2.2/wtpsplit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,29 +172,44 @@
             i = i + 1 + next(index for index, label in enumerate(labels[i + 1 :]) if label != 0)
         except StopIteration:
             break
 
     return input_ids, block_ids, labels
 
 
-def indices_to_sentences(text, indices):
+def indices_to_sentences(text, indices, strip_whitespace=False):
     sentences = []
 
     offset = 0
     idx = 0
     for idx in indices:
         idx = idx + 1
         while idx < len(text) and text[idx].isspace():
             idx += 1
 
-        sentences.append(text[offset:idx])
+        sentence = text[offset:idx]
+        if strip_whitespace:
+            # NB: I would have thought that this is slower than
+            # adjusting the start and end indices since there are
+            # two string copies, but it seems to be faster
+            # (at least on short strings). more reason to port to Rust?
+            sentence = sentence.strip()
+
+        if len(sentence) > 0:
+            sentences.append(sentence)
+
         offset = idx
 
     if idx != len(text):
-        sentences.append(text[idx:])
+        last_sentence = text[idx:]
+        if strip_whitespace:
+            last_sentence = last_sentence.strip()
+
+        if len(last_sentence) > 0:
+            sentences.append(last_sentence)
 
     return sentences
 
 
 def reconstruct_sentences(text, partial_sentences):
     # for consistency
     partial_sentences = [x.strip() for x in partial_sentences]
```

