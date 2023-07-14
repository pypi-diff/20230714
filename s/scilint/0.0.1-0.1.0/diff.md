# Comparing `tmp/scilint-0.0.1.tar.gz` & `tmp/scilint-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilint-0.0.1.tar", last modified: Wed Jun 28 20:07:21 2023, max compression
+gzip compressed data, was "scilint-0.1.0.tar", last modified: Fri Jul 14 15:42:38 2023, max compression
```

## Comparing `scilint-0.0.1.tar` & `scilint-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:07:21.699120 scilint-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-28 20:06:01.000000 scilint-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-28 20:06:01.000000 scilint-0.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-06-28 20:07:21.699120 scilint-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-28 20:07:08.000000 scilint-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-28 20:06:01.000000 scilint-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:07:21.699120 scilint-0.0.1/scilint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 20:06:58.000000 scilint-0.0.1/scilint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-06-28 20:07:08.000000 scilint-0.0.1/scilint/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-06-28 20:06:58.000000 scilint-0.0.1/scilint/scilint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:07:21.699120 scilint-0.0.1/scilint/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 20:06:58.000000 scilint-0.0.1/scilint/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-28 20:06:58.000000 scilint-0.0.1/scilint/test/test_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-28 20:06:58.000000 scilint-0.0.1/scilint/test/test_nbdev_high_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:07:21.699120 scilint-0.0.1/scilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-06-28 20:07:21.000000 scilint-0.0.1/scilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-28 20:07:21.000000 scilint-0.0.1/scilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 20:07:21.000000 scilint-0.0.1/scilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-28 20:07:21.000000 scilint-0.0.1/scilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 20:06:15.000000 scilint-0.0.1/scilint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-28 20:07:21.000000 scilint-0.0.1/scilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 20:07:21.000000 scilint-0.0.1/scilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 20:07:21.699120 scilint-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-28 20:06:01.000000 scilint-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-14 15:41:07.000000 scilint-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-14 15:41:07.000000 scilint-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-14 15:42:38.072636 scilint-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17401 2023-07-14 15:42:22.000000 scilint-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-14 15:41:07.000000 scilint-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.068636 scilint-0.1.0/scilint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25902 2023-07-14 15:42:22.000000 scilint-0.1.0/scilint/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/experimental/test_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/exploratory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/exploratory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/exploratory/test_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22180 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/scilint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/test/test_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/test/test_nbdev_high_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint/validated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:07.000000 scilint-0.1.0/scilint/validated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 15:42:06.000000 scilint-0.1.0/scilint/validated/test_nbdev_high_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:42:38.072636 scilint-0.1.0/scilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:41:20.000000 scilint-0.1.0/scilint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 15:42:38.000000 scilint-0.1.0/scilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:42:38.072636 scilint-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-14 15:41:07.000000 scilint-0.1.0/setup.py
```

### Comparing `scilint-0.0.1/LICENSE` & `scilint-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scilint-0.0.1/NOTICE` & `scilint-0.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `scilint-0.0.1/scilint/test/test_nbdev.py` & `scilint-0.1.0/scilint/experimental/test_nbdev.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/example_nbs/nbdev.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/example_nbs/experimental/nbdev.ipynb.
 
 # %% auto 0
 __all__ = ['traffic_percent', 'workers', 'model_level', 'min_date', 'something', 'get_traffic_text', 'get_experiment_segment',
            'get_utterances', 'preprocess', 'Topics', 'fit', 'evaluate', 'serve_num_topics']
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 2
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 2
 def something():
     message = "The first step"
     print(f"{message}")
     results = {"message": message}
     return results
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 6
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 6
 import numpy as np
 import pandas as pd
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 8
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 8
 traffic_percent = 1
 workers = 8
 model_level = "dispatcher"
 min_date = "2021-01-01"
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 9
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 9
 def get_traffic_text(percent):
     return str(percent) if int(percent) >= 10 else "0" + str(percent)
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 15
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 15
 def get_experiment_segment(traffic_percent):
     return tuple(get_traffic_text(tp) for tp in range(traffic_percent))
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 17
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 17
 def get_utterances(model_level=None, min_date=None, traffic_percent=100):
     """
     You will probably call data preparation code here. To simplify dependencies we are just creating synthetic data instead.
     """
     get_experiment_segment(traffic_percent)
     dummy_data = pd.Series(
         np.random.choice(
@@ -46,23 +46,23 @@
             ],
             100,
         ),
         name="utterance",
     )
     return dummy_data
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 18
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 18
 def preprocess(message, model_level=None, min_date=None, traffic_percent=100):
     print(f"I captialised the message: {message.upper()}")
     data = get_utterances(model_level, min_date, traffic_percent)
     documents = data.tolist()
     results = {"documents": documents}
     return results
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 21
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 21
 class Topics:
     def __init__(self, documents, workers):
         pass
 
     def get_num_topics(self):
         return 6
 
@@ -75,21 +75,21 @@
             np.asarray([1, 1, 1, 1, 1, 1]),
             [1, 2, 3, 4, 5, 6],
         )
 
     def plot_wordcloud(self):
         print("you may want to remove plotting code from testing to speed things up")
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 23
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 23
 def fit(documents, workers=workers):
     model = Topics(documents, workers=workers)
     results = {"model": model}
     return results
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 35
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 35
 def evaluate(model):
     topic_words, word_scores, topic_nums = model.get_topics(model.get_num_topics())
 
     topic_contains_non_empty_words = all([len(tw) > 0 for tw in topic_words])
     word_scores_in_range = word_scores.min() >= 0.0 and word_scores.max() <= 1.0
     as_many_items_as_topics = (
         model.get_num_topics() == len(topic_words) == word_scores.shape[0]
@@ -111,10 +111,10 @@
     results = {
         "word_summaries": word_summaries,
         "artifacts": artifacts,
         "metrics": metrics,
     }
     return results
 
-# %% ../../nbs/example_nbs/nbdev.ipynb 38
+# %% ../../nbs/example_nbs/experimental/nbdev.ipynb 38
 def serve_num_topics(model):
     return model.get_num_topics()
```

### Comparing `scilint-0.0.1/scilint/test/test_nbdev_high_quality.py` & `scilint-0.1.0/scilint/test/test_nbdev_high_quality.py`

 * *Files identical despite different names*

### Comparing `scilint-0.0.1/setup.py` & `scilint-0.1.0/setup.py`

 * *Files identical despite different names*

