# Comparing `tmp/dicee-0.0.3.tar.gz` & `tmp/dicee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicee-0.0.3.tar", last modified: Wed May  3 09:09:26 2023, max compression
+gzip compressed data, was "dicee-0.0.4.tar", last modified: Fri Jul 14 10:18:38 2023, max compression
```

## Comparing `dicee-0.0.3.tar` & `dicee-0.0.4.tar`

### file list

```diff
@@ -1,109 +1,113 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.520754 dicee-0.0.3/
--rw-rw-r--   0 demir     (1000) demir     (1000)    10829 2023-02-28 08:40:45.000000 dicee-0.0.3/Kronecker_classes.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    34522 2022-06-06 08:52:00.000000 dicee-0.0.3/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)      173 2023-02-17 09:26:52.000000 dicee-0.0.3/MANIFEST.in
--rw-rw-r--   0 demir     (1000) demir     (1000)    10701 2023-05-03 09:09:26.516754 dicee-0.0.3/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)    10235 2023-04-03 11:09:14.000000 dicee-0.0.3/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)     4690 2023-03-16 15:06:38.000000 dicee-0.0.3/analyse_experiments.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1585 2023-02-17 09:26:52.000000 dicee-0.0.3/continual_training.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.492754 dicee-0.0.3/dicee/
--rw-rw-r--   0 demir     (1000) demir     (1000)      185 2023-03-16 12:08:33.000000 dicee-0.0.3/dicee/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    13471 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/abstracts.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    10250 2023-04-03 11:09:14.000000 dicee-0.0.3/dicee/callbacks.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1419 2023-03-16 12:08:33.000000 dicee-0.0.3/dicee/config.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    19069 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/dataset_classes.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    18972 2023-03-14 12:57:41.000000 dicee-0.0.3/dicee/evaluator.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    14599 2023-03-21 19:46:38.000000 dicee-0.0.3/dicee/executer.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.492754 dicee-0.0.3/dicee/figures/
--rw-rw-r--   0 demir     (1000) demir     (1000)   168919 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/figures/deploy_qmult_family.png
--rw-rw-r--   0 demir     (1000) demir     (1000)     4838 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/helper_classes.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     3513 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/knowledge_graph.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    24330 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/knowledge_graph_embeddings.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.496754 dicee-0.0.3/dicee/models/
--rw-rw-r--   0 demir     (1000) demir     (1000)      192 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/models/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    15522 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/models/base_model.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    29747 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/models/clifford.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    15883 2023-03-24 17:49:01.000000 dicee-0.0.3/dicee/models/complex.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    10805 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/models/function_space.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    14842 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/models/octonion.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    12082 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/models/quaternion.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     6075 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/models/real.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      562 2023-02-17 14:37:00.000000 dicee-0.0.3/dicee/models/static_funcs.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.500754 dicee-0.0.3/dicee/read_preprocess_save_load_kg/
--rw-rw-r--   0 demir     (1000) demir     (1000)      142 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/read_preprocess_save_load_kg/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    16606 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/read_preprocess_save_load_kg/preprocess.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1043 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/read_preprocess_save_load_kg/read_from_disk.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4069 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/read_preprocess_save_load_kg/save_load_disk.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    17232 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/read_preprocess_save_load_kg/util.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2191 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/sanity_checkers.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    24688 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/static_funcs.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      304 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/static_funcs_training.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4964 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/static_preprocess_funcs.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.500754 dicee-0.0.3/dicee/trainer/
--rw-rw-r--   0 demir     (1000) demir     (1000)       38 2023-02-17 09:26:52.000000 dicee-0.0.3/dicee/trainer/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    12065 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/trainer/dice_trainer.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     8143 2023-05-03 08:58:58.000000 dicee-0.0.3/dicee/trainer/torch_trainer.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    13246 2023-04-26 11:34:00.000000 dicee-0.0.3/dicee/trainer/torch_trainer_ddp.py
--rw-rw-r--   0 demir     (1000) demir     (1000)       88 2023-03-16 12:08:33.000000 dicee-0.0.3/dicee/types.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.492754 dicee-0.0.3/dicee.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)    10701 2023-05-03 09:09:26.000000 dicee-0.0.3/dicee.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     2615 2023-05-03 09:09:26.000000 dicee-0.0.3/dicee.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-03 09:09:26.000000 dicee-0.0.3/dicee.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)      147 2023-05-03 09:09:26.000000 dicee-0.0.3/dicee.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       12 2023-05-03 09:09:26.000000 dicee-0.0.3/dicee.egg-info/top_level.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)    20658 2023-04-28 11:58:24.000000 dicee-0.0.3/dl_learning.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.480754 dicee-0.0.3/documents/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.500754 dicee-0.0.3/documents/DBpedia_experiments/
--rw-rw-r--   0 demir     (1000) demir     (1000)     4513 2022-10-19 10:04:23.000000 dicee-0.0.3/documents/DBpedia_experiments/ReadMe.md
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.500754 dicee-0.0.3/documents/KGEonTabular/
--rw-rw-r--   0 demir     (1000) demir     (1000)     2972 2023-01-05 11:53:35.000000 dicee-0.0.3/documents/KGEonTabular/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)     3478 2023-01-05 11:53:35.000000 dicee-0.0.3/documents/KGEonTabular/regression.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.500754 dicee-0.0.3/documents/SoftwareBenchmarks/
--rw-rw-r--   0 demir     (1000) demir     (1000)     6359 2023-01-05 11:53:35.000000 dicee-0.0.3/documents/SoftwareBenchmarks/read_csv_bencmark.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.504754 dicee-0.0.3/documents/training_techniques/
--rw-rw-r--   0 demir     (1000) demir     (1000)      242 2022-08-08 09:52:02.000000 dicee-0.0.3/documents/training_techniques/1vsall.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       27 2022-08-08 09:52:02.000000 dicee-0.0.3/documents/training_techniques/kvsall.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       29 2022-08-08 09:52:02.000000 dicee-0.0.3/documents/training_techniques/negative_sampling.md
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.504754 dicee-0.0.3/documents/using_dice_embedding_framework/
--rw-rw-r--   0 demir     (1000) demir     (1000)     4837 2022-08-08 09:52:02.000000 dicee-0.0.3/documents/using_dice_embedding_framework/Training.md
--rw-rw-r--   0 demir     (1000) demir     (1000)     3202 2022-05-12 09:35:29.000000 dicee-0.0.3/environment.yml
--rw-rw-r--   0 demir     (1000) demir     (1000)    12326 2023-01-09 13:38:49.000000 dicee-0.0.3/example_class_combine_kge.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     8139 2023-03-09 21:06:37.000000 dicee-0.0.3/gpt.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     7023 2023-03-14 14:25:05.000000 dicee-0.0.3/large_file_preprocessing.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)     5328 2023-05-03 08:58:09.000000 dicee-0.0.3/main.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1955 2023-03-05 16:34:53.000000 dicee-0.0.3/meta_heuristic.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2569 2023-02-27 20:06:53.000000 dicee-0.0.3/out_of_sample.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2548 2023-03-07 08:23:10.000000 dicee-0.0.3/plot.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1806 2023-03-09 11:17:44.000000 dicee-0.0.3/self_attention.py
--rw-rw-r--   0 demir     (1000) demir     (1000)       38 2023-05-03 09:09:26.520754 dicee-0.0.3/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)     1052 2023-05-03 09:09:24.000000 dicee-0.0.3/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-03 09:09:26.516754 dicee-0.0.3/tests/
--rw-rw-r--   0 demir     (1000) demir     (1000)        0 2022-05-12 09:35:29.000000 dicee-0.0.3/tests/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1770 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_auto_batch_finder.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1460 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_conjuncive_query_answering.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2557 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_continual_training.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4975 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_custom_trainer.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1084 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_deployment.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1096 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_different_backends.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1471 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_ensemble_construction.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4926 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_execute_start.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      861 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_gradient_accumulation.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     6919 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_k_fold_cv_1_vs_all.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     6518 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_k_fold_cv_k_vs_all.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4687 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_k_fold_cv_neg_sample.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2202 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_kvssample.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2025 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_large_kg.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2210 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_online_learning.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2894 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_pickle.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2597 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_read_few_only.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1104 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_aconex.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1299 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_cl.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     3103 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_complex.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     3066 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_conex.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2553 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_convo.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2780 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_distmult.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     3153 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_omult.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2367 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_polyak.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      693 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_pyke.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     3581 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_regression_qmult.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1046 2023-04-26 11:34:00.000000 dicee-0.0.3/tests/test_trainers.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.625800 dicee-0.0.4/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    10829 2023-02-28 08:40:45.000000 dicee-0.0.4/Kronecker_classes.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    34522 2022-06-06 08:52:00.000000 dicee-0.0.4/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)      173 2023-02-17 09:26:52.000000 dicee-0.0.4/MANIFEST.in
+-rw-rw-r--   0 demir     (1000) demir     (1000)    11338 2023-07-14 10:18:38.625800 dicee-0.0.4/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)    10872 2023-07-14 09:59:41.000000 dicee-0.0.4/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4940 2023-07-11 09:01:47.000000 dicee-0.0.4/analyse_experiments.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1585 2023-02-17 09:26:52.000000 dicee-0.0.4/continual_training.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.609800 dicee-0.0.4/dicee/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      185 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    13565 2023-07-14 09:52:30.000000 dicee-0.0.4/dicee/abstracts.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    10252 2023-07-14 09:52:30.000000 dicee-0.0.4/dicee/callbacks.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2034 2023-07-14 09:52:30.000000 dicee-0.0.4/dicee/config.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    19069 2023-07-13 10:44:46.000000 dicee-0.0.4/dicee/dataset_classes.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    18972 2023-07-11 15:21:33.000000 dicee-0.0.4/dicee/evaluator.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    14939 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/executer.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.609800 dicee-0.0.4/dicee/figures/
+-rw-rw-r--   0 demir     (1000) demir     (1000)   168919 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/figures/deploy_qmult_family.png
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4838 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/helper_classes.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3513 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/knowledge_graph.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    24319 2023-07-13 18:48:59.000000 dicee-0.0.4/dicee/knowledge_graph_embeddings.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)   105541 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/lp.png
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.613800 dicee-0.0.4/dicee/models/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      201 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/models/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    15544 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/models/base_model.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    29747 2023-07-14 09:28:31.000000 dicee-0.0.4/dicee/models/clifford.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    15883 2023-03-24 17:49:01.000000 dicee-0.0.4/dicee/models/complex.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    10806 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/models/function_space.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    23078 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/models/octonion.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5974 2023-07-14 09:52:30.000000 dicee-0.0.4/dicee/models/pykeen_models.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    18227 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/models/quaternion.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     6075 2023-06-19 13:01:15.000000 dicee-0.0.4/dicee/models/real.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      562 2023-02-17 14:37:00.000000 dicee-0.0.4/dicee/models/static_funcs.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.613800 dicee-0.0.4/dicee/read_preprocess_save_load_kg/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      142 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/read_preprocess_save_load_kg/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    16606 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/read_preprocess_save_load_kg/preprocess.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1043 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/read_preprocess_save_load_kg/read_from_disk.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4069 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/read_preprocess_save_load_kg/save_load_disk.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    15525 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/read_preprocess_save_load_kg/util.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2191 2023-05-12 09:18:05.000000 dicee-0.0.4/dicee/sanity_checkers.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    26381 2023-07-14 09:52:30.000000 dicee-0.0.4/dicee/static_funcs.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      304 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/static_funcs_training.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4964 2023-04-26 11:34:00.000000 dicee-0.0.4/dicee/static_preprocess_funcs.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.617800 dicee-0.0.4/dicee/trainer/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       38 2023-02-17 09:26:52.000000 dicee-0.0.4/dicee/trainer/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    12184 2023-07-14 09:52:30.000000 dicee-0.0.4/dicee/trainer/dice_trainer.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     8143 2023-07-11 15:06:22.000000 dicee-0.0.4/dicee/trainer/torch_trainer.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    13246 2023-07-11 09:01:47.000000 dicee-0.0.4/dicee/trainer/torch_trainer_ddp.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)       88 2023-03-16 12:08:33.000000 dicee-0.0.4/dicee/types.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.609800 dicee-0.0.4/dicee.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    11338 2023-07-14 10:18:38.000000 dicee-0.0.4/dicee.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2688 2023-07-14 10:18:38.000000 dicee-0.0.4/dicee.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-07-14 10:18:38.000000 dicee-0.0.4/dicee.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)      180 2023-07-14 10:18:38.000000 dicee-0.0.4/dicee.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       12 2023-07-14 10:18:38.000000 dicee-0.0.4/dicee.egg-info/top_level.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)    41735 2023-05-16 08:06:02.000000 dicee-0.0.4/dl_learning.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.601800 dicee-0.0.4/documents/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.617800 dicee-0.0.4/documents/DBpedia_experiments/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4513 2023-05-12 09:06:07.000000 dicee-0.0.4/documents/DBpedia_experiments/ReadMe.md
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.617800 dicee-0.0.4/documents/KGEonTabular/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2972 2023-01-05 11:53:35.000000 dicee-0.0.4/documents/KGEonTabular/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3478 2023-07-11 09:01:47.000000 dicee-0.0.4/documents/KGEonTabular/regression.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.617800 dicee-0.0.4/documents/SoftwareBenchmarks/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     6359 2023-01-05 11:53:35.000000 dicee-0.0.4/documents/SoftwareBenchmarks/read_csv_bencmark.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.617800 dicee-0.0.4/documents/training_techniques/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      242 2022-08-08 09:52:02.000000 dicee-0.0.4/documents/training_techniques/1vsall.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       27 2022-08-08 09:52:02.000000 dicee-0.0.4/documents/training_techniques/kvsall.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       29 2022-08-08 09:52:02.000000 dicee-0.0.4/documents/training_techniques/negative_sampling.md
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.617800 dicee-0.0.4/documents/using_dice_embedding_framework/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4837 2022-08-08 09:52:02.000000 dicee-0.0.4/documents/using_dice_embedding_framework/Training.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)      292 2023-07-13 18:49:17.000000 dicee-0.0.4/dummy.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3202 2022-05-12 09:35:29.000000 dicee-0.0.4/environment.yml
+-rw-rw-r--   0 demir     (1000) demir     (1000)    12326 2023-01-09 13:38:49.000000 dicee-0.0.4/example_class_combine_kge.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     8139 2023-03-09 21:06:37.000000 dicee-0.0.4/gpt.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     7023 2023-03-14 14:25:05.000000 dicee-0.0.4/large_file_preprocessing.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5632 2023-07-14 09:52:30.000000 dicee-0.0.4/main.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1955 2023-03-05 16:34:53.000000 dicee-0.0.4/meta_heuristic.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2569 2023-02-27 20:06:53.000000 dicee-0.0.4/out_of_sample.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2626 2023-05-12 08:28:09.000000 dicee-0.0.4/plot.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1806 2023-03-09 11:17:44.000000 dicee-0.0.4/self_attention.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)       38 2023-07-14 10:18:38.625800 dicee-0.0.4/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1004 2023-07-14 10:18:36.000000 dicee-0.0.4/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-07-14 10:18:38.625800 dicee-0.0.4/tests/
+-rw-rw-r--   0 demir     (1000) demir     (1000)        0 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1770 2023-04-26 11:34:00.000000 dicee-0.0.4/tests/test_auto_batch_finder.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1434 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_conjuncive_query_answering.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2505 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_continual_training.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4793 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_custom_trainer.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1944 2023-07-14 09:52:30.000000 dicee-0.0.4/tests/test_deployment.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1070 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_different_backends.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1445 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_ensemble_construction.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4729 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_execute_start.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      832 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_gradient_accumulation.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     6687 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_k_fold_cv_1_vs_all.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     6292 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_k_fold_cv_k_vs_all.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4487 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_k_fold_cv_neg_sample.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2144 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_kvssample.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1967 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_large_kg.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2181 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_online_learning.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2778 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_pickle.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2964 2023-07-14 09:52:30.000000 dicee-0.0.4/tests/test_pykeen.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2568 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_read_few_only.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1075 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_aconex.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1270 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_cl.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3016 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_complex.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3033 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_conex.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2466 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_convo.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2693 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_distmult.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3066 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_omult.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2309 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_polyak.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      664 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_pyke.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3494 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_regression_qmult.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      988 2023-07-11 09:01:47.000000 dicee-0.0.4/tests/test_trainers.py
```

### Comparing `dicee-0.0.3/Kronecker_classes.py` & `dicee-0.0.4/Kronecker_classes.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/LICENSE` & `dicee-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/PKG-INFO` & `dicee-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dicee
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dice embedding is an hardware-agnostic framework for large-scale knowledge graph embedding applications
 Home-page: https://github.com/dice-group/dice-embeddings
 Author: Caglar Demir
 Author-email: caglardemir8@gmail.com
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DICE Embeddings: Hardware-agnostic Framework for Large-scale Knowledge Graph Embeddings
 
@@ -35,33 +35,37 @@
 Users can choose the trainer class (e.g., DDP by Pytorch) to train large knowledge graph embedding models with billions of parameters.
 PytorchLightning allows us to use state-of-the-art model parallelism techniques (e.g. Fully Sharded Training, FairScale, or DeepSpeed)
 without extra effort.
 With our framework, practitioners can directly use PytorchLightning for model parallelism to train gigantic embedding models.
 
 **Why [Hugging-face Gradio](https://huggingface.co/gradio)?**
 Deploy a pre-trained embedding model without writing a single line of code.
+# Installation
+<details><summary> Details </summary>
 
-
-## Installation
-```
+``` 
 pip install dicee
 ```
+
 or
+
 ```
 git clone https://github.com/dice-group/dice-embeddings.git
 conda create -n dice python=3.10 --no-default-packages && conda activate dice
 pip3 install "pandas>=1.5.1"
 pip3 install "torch>=2.0.0"
 pip3 install "polars>=0.16.14"
 pip3 install "scikit-learn>=1.2.2"
 pip3 install "pyarrow>=11.0.0"
 pip3 install "pytest>=7.2.2"
 pip3 install "gradio>=3.23.0"
 pip3 install "psutil>=5.9.4"
 pip3 install "pytorch-lightning==1.6.4"
+pip3 install "pykeen==1.10.1"
+pip3 install "zstandard>=0.21.0"
 ```
 To test the Installation
 ```
 wget https://hobbitdata.informatik.uni-leipzig.de/KG/KGs.zip
 unzip KGs.zip
 pytest -p no:warnings -x # it takes circa 15 minutes
 pytest -p no:warnings --lf # run only the last failed test
@@ -69,35 +73,42 @@
 ```
 To see the software architecture, execute the following command
 ```
 pyreverse dicee/ && dot -Tpng -x classes.dot -o dice_software.png && eog dice_software.png
 # or
 pyreverse dicee/trainer && dot -Tpng -x classes.dot -o trainer.png && eog trainer.png
 ```
-## Applications
-### Description Logic Concept Learning (soon)
-```python
-from dicee import KGE
-# (1) Load a pretrained KGE model on KGs/Family
-pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
-pretrained_model.learn_concepts(pos={''},neg={''},topk=1)
-```
-### Conjunctive Query/Question Answering
+</details>
+
+# Knowledge Graph Embedding Models
+<details> <summary> Details</summary>
+
+1. TransE, DistMult, ComplEx, ConEx, QMult, OMult, ConvO, ConvQ, Keci
+2. All 44 models available in https://github.com/pykeen/pykeen#models
+
+> For more, please refer to `examples`.
+</details>
+
+# How to Train
+<details> <summary> Details</summary>
+
+> Please refer to `examples`.
+</details>
+
+
+# How to Deploy
 ```python
 from dicee import KGE
-# (1) Load a pretrained KGE model on KGs/Family
-pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
-# (2) Answer the following conjunctive query question: To whom a sibling of F9M167 is married to?
-# (3) Decompose (2) into two query
-# (3.1) Who is a sibling of F9M167? => {F9F141,F9M157}
-# (3.2) To whom a results of (3.1) is married to ? {F9M142, F9F158}
-pretrained_model.predict_conjunctive_query(entity='<http://www.benchmark.org/family#F9M167>',
-                                          relations=['<http://www.benchmark.org/family#hasSibling>',
-                                                     '<http://www.benchmark.org/family#married>'], topk=1)
+KGE(path='...').deploy(share=True,top_k=10)
 ```
+<details> <summary> To see the interface of the webservice</summary>
+<img src="dicee/lp.png" alt="Italian Trulli">
+</details>
+
+## Downstream Applications
 ### Triple Classification
 #### Using pre-trained ConEx on DBpedia 03-2022
 ```bash
 # To download a pretrained ConEx
 mkdir ConEx && cd ConEx && wget -r -nd -np https://hobbitdata.informatik.uni-leipzig.de/KGE/DBpedia/ConEx/ && cd ..
 ```
 ```python
@@ -127,25 +138,38 @@
 ```
 ### Finding Missing Triples
 ```python
 from dicee import KGE
 pre_trained_kge = KGE(path='ConEx')
 missing_triples = pre_trained_kge.find_missing_triples(confidence=0.95, entities=[''], relations=[''])
 ```
+### Complex Query Answering
+The beam search technique proposed in [Complex Query Answering with Neural Link Predictors](https://arxiv.org/abs/2011.03459)
+```python
+from dicee import KGE
+# (1) Load a pretrained KGE model on KGs/Family
+pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
+# (2) Query: ?P : \exist Married(P,E) \land hasSibling(E, F9M167) (To whom a sibling of F9M167 is married to?   
+# (3) Decompose (2) into two query
+# (3.1) Who is a sibling of F9M167? => hasSibling(E, F9M167) => {F9F141,F9M157}
+# (3.2) To whom a results of (3.1) is married to ? {F9M142, F9F158}
+pretrained_model.predict_conjunctive_query(entity='<http://www.benchmark.org/family#F9M167>',
+                                          relations=['<http://www.benchmark.org/family#hasSibling>',
+                                                     '<http://www.benchmark.org/family#married>'], topk=1)
+```
 
-## How to Train a KGE model 
-> How to use the framework:`examples`.
-
-## How to Deploy
-Any pretrained model can be deployed with an ease. By setting ```share=True```, anyone on the internet can use a pretrained model.
+### Description Logic Concept Learning (soon)
 ```python
 from dicee import KGE
-KGE(path='...').deploy(share=True,top_k=10)
+# (1) Load a pretrained KGE model on KGs/Family
+pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
+pretrained_model.learn_concepts(pos={''},neg={''},topk=1)
 ```
-![alt text](dicee/figures/deploy_qmult_family.png)
+
+
 ## Pre-trained Models
 Please contact:  ```caglar.demir@upb.de ``` or ```caglardemir8@gmail.com ``` , if you lack hardware resources to obtain embeddings of a specific knowledge Graph.
 - [DBpedia version: 06-2022 Embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/DBpediaQMultEmbeddings_03_07):
   - Models: ConEx, QMult
 - [YAGO3-10 ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/YAGO3-10.zip)
 - [FB15K-237 ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/FB15K-237.zip)
 - [WN18RR ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/WN18RR.zip)
@@ -161,19 +185,22 @@
 @article{demir2022hardware,
   title={Hardware-agnostic computation for large-scale knowledge graph embeddings},
   author={Demir, Caglar and Ngomo, Axel-Cyrille Ngonga},
   journal={Software Impacts},
   year={2022},
   publisher={Elsevier}
 }
+# Keci
+Accepted at ECML. Stay tuned for the manuscript!
 # KronE
-@article{demir2022kronecker,
-  title={Kronecker Decomposition for Knowledge Graph Embeddings},
-  author={Demir, Caglar and Lienen, Julian and Ngomo, Axel-Cyrille Ngonga},
-  journal={arXiv preprint arXiv:2205.06560},
+@inproceedings{demir2022kronecker,
+  title={Kronecker decomposition for knowledge graph embeddings},
+  author={Demir, Caglar and Lienen, Julian and Ngonga Ngomo, Axel-Cyrille},
+  booktitle={Proceedings of the 33rd ACM Conference on Hypertext and Social Media},
+  pages={1--10},
   year={2022}
 }
 # QMult, OMult, ConvQ, ConvO
 @InProceedings{pmlr-v157-demir21a,
   title = 	 {Convolutional Hypercomplex Embeddings for Link Prediction},
   author =       {Demir, Caglar and Moussallem, Diego and Heindorf, Stefan and Ngonga Ngomo, Axel-Cyrille},
   booktitle = 	 {Proceedings of The 13th Asian Conference on Machine Learning},
```

### Comparing `dicee-0.0.3/README.md` & `dicee-0.0.4/dicee.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: dicee
+Version: 0.0.4
+Summary: Dice embedding is an hardware-agnostic framework for large-scale knowledge graph embedding applications
+Home-page: https://github.com/dice-group/dice-embeddings
+Author: Caglar Demir
+Author-email: caglardemir8@gmail.com
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DICE Embeddings: Hardware-agnostic Framework for Large-scale Knowledge Graph Embeddings
 
 Knowledge graph embedding research has mainly focused on learning continuous representations of knowledge graphs towards the link prediction problem. 
 Recently developed frameworks can be effectively applied in a wide range of research-related applications.
 Yet, using these frameworks in real-world applications becomes more challenging as the size of the knowledge graph grows.
 
 We developed the DICE Embeddings framework (dicee) to compute embeddings for large-scale knowledge graphs in a hardware-agnostic manner.
@@ -22,33 +35,37 @@
 Users can choose the trainer class (e.g., DDP by Pytorch) to train large knowledge graph embedding models with billions of parameters.
 PytorchLightning allows us to use state-of-the-art model parallelism techniques (e.g. Fully Sharded Training, FairScale, or DeepSpeed)
 without extra effort.
 With our framework, practitioners can directly use PytorchLightning for model parallelism to train gigantic embedding models.
 
 **Why [Hugging-face Gradio](https://huggingface.co/gradio)?**
 Deploy a pre-trained embedding model without writing a single line of code.
+# Installation
+<details><summary> Details </summary>
 
-
-## Installation
-```
+``` 
 pip install dicee
 ```
+
 or
+
 ```
 git clone https://github.com/dice-group/dice-embeddings.git
 conda create -n dice python=3.10 --no-default-packages && conda activate dice
 pip3 install "pandas>=1.5.1"
 pip3 install "torch>=2.0.0"
 pip3 install "polars>=0.16.14"
 pip3 install "scikit-learn>=1.2.2"
 pip3 install "pyarrow>=11.0.0"
 pip3 install "pytest>=7.2.2"
 pip3 install "gradio>=3.23.0"
 pip3 install "psutil>=5.9.4"
 pip3 install "pytorch-lightning==1.6.4"
+pip3 install "pykeen==1.10.1"
+pip3 install "zstandard>=0.21.0"
 ```
 To test the Installation
 ```
 wget https://hobbitdata.informatik.uni-leipzig.de/KG/KGs.zip
 unzip KGs.zip
 pytest -p no:warnings -x # it takes circa 15 minutes
 pytest -p no:warnings --lf # run only the last failed test
@@ -56,35 +73,42 @@
 ```
 To see the software architecture, execute the following command
 ```
 pyreverse dicee/ && dot -Tpng -x classes.dot -o dice_software.png && eog dice_software.png
 # or
 pyreverse dicee/trainer && dot -Tpng -x classes.dot -o trainer.png && eog trainer.png
 ```
-## Applications
-### Description Logic Concept Learning (soon)
-```python
-from dicee import KGE
-# (1) Load a pretrained KGE model on KGs/Family
-pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
-pretrained_model.learn_concepts(pos={''},neg={''},topk=1)
-```
-### Conjunctive Query/Question Answering
+</details>
+
+# Knowledge Graph Embedding Models
+<details> <summary> Details</summary>
+
+1. TransE, DistMult, ComplEx, ConEx, QMult, OMult, ConvO, ConvQ, Keci
+2. All 44 models available in https://github.com/pykeen/pykeen#models
+
+> For more, please refer to `examples`.
+</details>
+
+# How to Train
+<details> <summary> Details</summary>
+
+> Please refer to `examples`.
+</details>
+
+
+# How to Deploy
 ```python
 from dicee import KGE
-# (1) Load a pretrained KGE model on KGs/Family
-pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
-# (2) Answer the following conjunctive query question: To whom a sibling of F9M167 is married to?
-# (3) Decompose (2) into two query
-# (3.1) Who is a sibling of F9M167? => {F9F141,F9M157}
-# (3.2) To whom a results of (3.1) is married to ? {F9M142, F9F158}
-pretrained_model.predict_conjunctive_query(entity='<http://www.benchmark.org/family#F9M167>',
-                                          relations=['<http://www.benchmark.org/family#hasSibling>',
-                                                     '<http://www.benchmark.org/family#married>'], topk=1)
+KGE(path='...').deploy(share=True,top_k=10)
 ```
+<details> <summary> To see the interface of the webservice</summary>
+<img src="dicee/lp.png" alt="Italian Trulli">
+</details>
+
+## Downstream Applications
 ### Triple Classification
 #### Using pre-trained ConEx on DBpedia 03-2022
 ```bash
 # To download a pretrained ConEx
 mkdir ConEx && cd ConEx && wget -r -nd -np https://hobbitdata.informatik.uni-leipzig.de/KGE/DBpedia/ConEx/ && cd ..
 ```
 ```python
@@ -114,25 +138,38 @@
 ```
 ### Finding Missing Triples
 ```python
 from dicee import KGE
 pre_trained_kge = KGE(path='ConEx')
 missing_triples = pre_trained_kge.find_missing_triples(confidence=0.95, entities=[''], relations=[''])
 ```
+### Complex Query Answering
+The beam search technique proposed in [Complex Query Answering with Neural Link Predictors](https://arxiv.org/abs/2011.03459)
+```python
+from dicee import KGE
+# (1) Load a pretrained KGE model on KGs/Family
+pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
+# (2) Query: ?P : \exist Married(P,E) \land hasSibling(E, F9M167) (To whom a sibling of F9M167 is married to?   
+# (3) Decompose (2) into two query
+# (3.1) Who is a sibling of F9M167? => hasSibling(E, F9M167) => {F9F141,F9M157}
+# (3.2) To whom a results of (3.1) is married to ? {F9M142, F9F158}
+pretrained_model.predict_conjunctive_query(entity='<http://www.benchmark.org/family#F9M167>',
+                                          relations=['<http://www.benchmark.org/family#hasSibling>',
+                                                     '<http://www.benchmark.org/family#married>'], topk=1)
+```
 
-## How to Train a KGE model 
-> How to use the framework:`examples`.
-
-## How to Deploy
-Any pretrained model can be deployed with an ease. By setting ```share=True```, anyone on the internet can use a pretrained model.
+### Description Logic Concept Learning (soon)
 ```python
 from dicee import KGE
-KGE(path='...').deploy(share=True,top_k=10)
+# (1) Load a pretrained KGE model on KGs/Family
+pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
+pretrained_model.learn_concepts(pos={''},neg={''},topk=1)
 ```
-![alt text](dicee/figures/deploy_qmult_family.png)
+
+
 ## Pre-trained Models
 Please contact:  ```caglar.demir@upb.de ``` or ```caglardemir8@gmail.com ``` , if you lack hardware resources to obtain embeddings of a specific knowledge Graph.
 - [DBpedia version: 06-2022 Embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/DBpediaQMultEmbeddings_03_07):
   - Models: ConEx, QMult
 - [YAGO3-10 ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/YAGO3-10.zip)
 - [FB15K-237 ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/FB15K-237.zip)
 - [WN18RR ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/WN18RR.zip)
@@ -148,19 +185,22 @@
 @article{demir2022hardware,
   title={Hardware-agnostic computation for large-scale knowledge graph embeddings},
   author={Demir, Caglar and Ngomo, Axel-Cyrille Ngonga},
   journal={Software Impacts},
   year={2022},
   publisher={Elsevier}
 }
+# Keci
+Accepted at ECML. Stay tuned for the manuscript!
 # KronE
-@article{demir2022kronecker,
-  title={Kronecker Decomposition for Knowledge Graph Embeddings},
-  author={Demir, Caglar and Lienen, Julian and Ngomo, Axel-Cyrille Ngonga},
-  journal={arXiv preprint arXiv:2205.06560},
+@inproceedings{demir2022kronecker,
+  title={Kronecker decomposition for knowledge graph embeddings},
+  author={Demir, Caglar and Lienen, Julian and Ngonga Ngomo, Axel-Cyrille},
+  booktitle={Proceedings of the 33rd ACM Conference on Hypertext and Social Media},
+  pages={1--10},
   year={2022}
 }
 # QMult, OMult, ConvQ, ConvO
 @InProceedings{pmlr-v157-demir21a,
   title = 	 {Convolutional Hypercomplex Embeddings for Link Prediction},
   author =       {Demir, Caglar and Moussallem, Diego and Heindorf, Stefan and Ngonga Ngomo, Axel-Cyrille},
   booktitle = 	 {Proceedings of The 13th Asian Conference on Machine Learning},
```

### Comparing `dicee-0.0.3/analyse_experiments.py` & `dicee-0.0.4/analyse_experiments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import pandas as pd
-
 import sys
 
+
 # print('Number of arguments:', len(sys.argv), 'arguments.')
 # print('Argument List:', str(sys.argv))
 
 
 if len(sys.argv) > 1:
     input_str_path = sys.argv[1]
 else:
@@ -32,15 +32,15 @@
     except:
         print('Exception occured at reading config')
         continue
 
     try:
         with open(input_str_path + path + '/report.json', 'r') as f:
             report = json.load(f)
-            report = {i: report[i] for i in ['Runtime']}
+            report = {i: report[i] for i in ['Runtime','NumParam']}
     except:
         print('Exception occured at reading report')
         continue
 
     try:
         with open(input_str_path + path + '/eval_report.json', 'r') as f:
             eval_report = json.load(f)
@@ -61,14 +61,15 @@
 
 # need a class to hold all params
 class Experiment:
     def __init__(self):
         self.model_name = []
         self.callbacks = []
         self.embedding_dim = []
+        self.num_params=[]
         self.num_epochs = []
         self.batch_size = []
         self.lr = []
         self.path_dataset_folder = []
         self.full_storage_path = []
         self.pq = []
         self.train_mrr = []
@@ -94,14 +95,15 @@
         self.embedding_dim.append(x['embedding_dim'])
         self.num_epochs.append(x['num_epochs'])
         self.batch_size.append(x['batch_size'])
         self.lr.append(x['lr'])
         self.path_dataset_folder.append(x['path_dataset_folder'])
         self.pq.append((x['p'], x['q']))
         self.runtime.append(x['Runtime'])
+        self.num_params.append(x['NumParam'])
 
         self.normalization.append(x['normalization'])
         self.callbacks.append(x['callbacks'])
 
         self.train_mrr.append(x['Train']['MRR'])
         self.train_h1.append(x['Train']['H@1'])
         self.train_h3.append(x['Train']['H@3'])
@@ -118,28 +120,36 @@
         self.test_mrr.append(x['Test']['MRR'])
         self.test_h1.append(x['Test']['H@1'])
         self.test_h3.append(x['Test']['H@3'])
         self.test_h10.append(x['Test']['H@10'])
 
     def to_df(self):
         return pd.DataFrame(
-            dict(model_name=self.model_name, pq=self.pq, path_dataset_folder=self.path_dataset_folder,
+            dict(model_name=self.model_name, #pq=self.pq, path_dataset_folder=self.path_dataset_folder,
                  train_mrr=self.train_mrr, train_h1=self.train_h1,
                  train_h3=self.train_h3, train_h10=self.train_h10,
-                 full_storage_path=self.full_storage_path,
+                 #full_storage_path=self.full_storage_path,
                  val_mrr=self.val_mrr, val_h1=self.val_h1,
                  val_h3=self.val_h3, val_h10=self.val_h10,
                  test_mrr=self.test_mrr, test_h1=self.test_h1,
                  test_h3=self.test_h3, test_h10=self.test_h10,
-                 runtime=self.runtime, callbacks=self.callbacks, normalization=self.normalization,
-                 embeddingdim=self.embedding_dim)
+                 runtime=self.runtime,
+                 params=self.num_params
+                 #callbacks=self.callbacks,
+                 #normalization=self.normalization,
+                 #embeddingdim=self.embedding_dim
+                 )
         )
 
 
 counter = Experiment()
 
 for i in experiments:
     counter.save_experiment(i)
 
-pd.set_option("display.precision", 3)
+
 df = counter.to_df()
-print(df.to_latex(index=False))
+pd.set_option("display.precision", 3)
+#print(df)
+#print(df.to_latex(index=False,float_format="%.3f"))
+
+print(df.to_markdown(index=False))
```

### Comparing `dicee-0.0.3/continual_training.py` & `dicee-0.0.4/continual_training.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/abstracts.py` & `dicee-0.0.4/dicee/abstracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import math
 import os
 import datetime
 # import pandas.core.indexes.range
-from .static_funcs import load_model_ensemble, load_model, save_checkpoint_model,load_numpy
+from .static_funcs import load_model_ensemble, load_model, save_checkpoint_model, load_numpy
 from .static_preprocess_funcs import create_constraints
 import torch
 from typing import List, Tuple
 import pandas as pd
 import numpy as np
 import random
 from abc import ABC, abstractmethod
+import pytorch_lightning
 
 
 class AbstractTrainer:
     """
     Abstract class for Trainer class for knowledge graph embedding models
 
 
@@ -166,15 +167,15 @@
         self.relation_to_idx: dict
         assert list(self.entity_to_idx.values()) == list(range(0, len(self.entity_to_idx)))
         assert list(self.relation_to_idx.values()) == list(range(0, len(self.relation_to_idx)))
 
         self.idx_to_entity = {v: k for k, v in self.entity_to_idx.items()}
         self.idx_to_relations = {v: k for k, v in self.relation_to_idx.items()}
 
-        self.train_set=load_numpy(path=self.path + '/train_set.npy')
+        self.train_set = load_numpy(path=self.path + '/train_set.npy')
         if self.apply_semantic_constraint:
             self.domain_constraints_per_rel, self.range_constraints_per_rel, self.domain_per_rel, self.range_per_rel = create_constraints(
                 self.train_set)
 
     def get_domain_of_relation(self, rel: str) -> List[str]:
         x = [self.idx_to_entity[i] for i in self.domain_per_rel[self.relation_to_idx[rel]]]
         res = set(x)
@@ -221,20 +222,20 @@
     @property
     def name(self):
         return self.model.name
 
     def sample_entity(self, n: int) -> List[str]:
         assert isinstance(n, int)
         assert n >= 0
-        return random.sample(self.entity_to_idx.keys(), n)
+        return random.sample([i for i in self.entity_to_idx.keys()], n)
 
     def sample_relation(self, n: int) -> List[str]:
         assert isinstance(n, int)
         assert n >= 0
-        return random.sample(self.relation_to_idx.keys(), n)
+        return random.sample([i for i in self.relation_to_idx.keys()], n)
 
     def is_seen(self, entity: str = None, relation: str = None) -> bool:
         if entity is not None:
             return True if self.entity_to_idx.get(entity) else False
         if relation is not None:
             return True if self.relation_to_idx.get(relation) else False
 
@@ -335,15 +336,15 @@
         labels: object = torch.FloatTensor(labels)
         return x, labels
 
     def parameters(self):
         return self.model.parameters()
 
 
-class AbstractCallback(ABC):
+class AbstractCallback(ABC, pytorch_lightning.callbacks.Callback):
     """
     Abstract class for Callback class for knowledge graph embedding models
 
 
     Parameter
     ---------
 
@@ -411,15 +412,15 @@
 
         Returns
         ---------
         None
         """
         pass
 
-    def on_train_batch_end(self, trainer, model):
+    def on_train_batch_end(self, *args, **kwargs):
         """
         Call at the end of each mini-batch during the training.
 
 
         Parameter
         ---------
         trainer:
@@ -428,15 +429,15 @@
 
         Returns
         ---------
         None
         """
         pass
 
-    def on_fit_end(self, trainer, model):
+    def on_fit_end(self, *args, **kwargs):
         """
         Call at the end of the training.
 
         Parameter
         ---------
         trainer:
```

### Comparing `dicee-0.0.3/dicee/callbacks.py` & `dicee-0.0.4/dicee/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,18 @@
 
     def on_train_epoch_end(self, *args, **kwargs):
         pass
 
     def on_fit_end(self, *args, **kwargs):
         pass
 
-    def on_epoch_end(self, trainer, pl_module):
+    def on_epoch_end(self, model, trainer, **kwargs):
         if self.epoch_counter % self.every_x_epoch == 0 and self.epoch_counter > 1:
             print(f'\nStoring model {self.epoch_counter}...')
-            save_checkpoint_model(pl_module,
+            save_checkpoint_model(model,
                                   path=self.path + f'/model_at_{str(self.epoch_counter)}_epoch_{str(str(datetime.datetime.now()))}.pt')
         self.epoch_counter += 1
 
 
 class PseudoLabellingCallback(AbstractCallback):
     def __init__(self, data_module, kg, batch_size):
         super().__init__()
```

### Comparing `dicee-0.0.3/dicee/dataset_classes.py` & `dicee-0.0.4/dicee/dataset_classes.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/evaluator.py` & `dicee-0.0.4/dicee/evaluator.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/executer.py` & `dicee-0.0.4/dicee/executer.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         self.trained_model = None
         # (6) A variable is initialized for storing input data.
         self.dataset = None
         # (7) Store few data in memory for numerical results, e.g. runtime, H@1 etc.
         self.report = dict()
         # (8) Create an object to carry out link prediction evaluations
         self.evaluator = None  # e.g. Evaluator(self)
+        # (9) Execution start time
+        self.start_time = None
 
     def read_preprocess_index_serialize_data(self) -> None:
         """ Read & Preprocess & Index & Serialize Input Data
 
         (1) Read or load the data from disk into memory.
         (2) Store the statistics of the data.
 
@@ -71,14 +73,15 @@
         self.args, self.dataset = config_kge_sanity_checking(self.args, self.dataset)
         # (3) Store the stats
         self.args.num_entities = self.dataset.num_entities
         self.args.num_relations = self.dataset.num_relations
         self.report['num_train_triples'] = len(self.dataset.train_set)
         self.report['num_entities'] = self.dataset.num_entities
         self.report['num_relations'] = self.dataset.num_relations
+        self.report['runtime_kg_loading'] = time.time() - self.start_time
 
     def load_indexed_data(self) -> None:
         """ Load the indexed data from disk into memory
 
         Parameter
         ----------
 
@@ -126,15 +129,15 @@
                   full_storage_path=self.storage_path, save_as_csv=self.args.save_embeddings_as_csv)
 
         self.report['path_experiment_folder'] = self.storage_path
         self.report['num_entities'] = self.args.num_entities
         self.report['num_relations'] = self.args.num_relations
         self.report['path_experiment_folder'] = self.storage_path
 
-    def end(self, start_time, form_of_labelling) -> dict:
+    def end(self, form_of_labelling) -> dict:
         """
         End training
 
         (1) Store trained model.
         (2) Report runtimes.
         (3) Eval model if required.
 
@@ -144,28 +147,33 @@
         Returns
         -------
         A dict containing information about the training and/or evaluation
 
         """
         # (1) Save the model
         self.save_trained_model()
-        # (2) Update and inform the runtime
-        self.report['Runtime'] = time.time() - start_time
-        print(f"Total computation time: {self.report['Runtime']:.3f} seconds")
-        # (3) Store the report of training.
-        with open(self.args.full_storage_path + '/report.json', 'w') as file_descriptor:
-            json.dump(self.report, file_descriptor, indent=4)
-        # (4) Eval model and return eval results.
+        # (2) Report
+        self.write_report()
+        # (3) Eval model and return eval results.
         if self.args.eval_model is None:
+            self.write_report()
             return {**self.report}
         else:
             self.evaluator.eval(dataset=self.dataset, trained_model=self.trained_model,
                                 form_of_labelling=form_of_labelling)
+            self.write_report()
             return {**self.report, **self.evaluator.report}
 
+    def write_report(self):
+        # Report total runtime.
+        self.report['Runtime'] = time.time() - self.start_time
+        print(f"Total computation time: {self.report['Runtime']:.3f} seconds")
+        with open(self.args.full_storage_path + '/report.json', 'w') as file_descriptor:
+            json.dump(self.report, file_descriptor, indent=4)
+
     def start(self) -> dict:
         """
         Start training
 
         # (1) Loading the Data
         # (2) Create an evaluator object.
         # (3) Create a trainer object.
@@ -175,29 +183,31 @@
         ---------
 
         Returns
         -------
         A dict containing information about the training and/or evaluation
 
         """
-        start_time = time.time()
+        self.start_time = time.time()
         print(f"Start time:{datetime.datetime.now()}")
         # (1) Loading the Data
         #  Load the indexed data from disk or read a raw data from disk.
         self.load_indexed_data() if self.is_continual_training else self.read_preprocess_index_serialize_data()
         # (2) Create an evaluator object.
         self.evaluator = Evaluator(args=self.args)
         # (3) Create a trainer object.
         self.trainer = DICE_Trainer(args=self.args,
                                     is_continual_training=self.is_continual_training,
                                     storage_path=self.storage_path,
-                                    evaluator=self.evaluator)
+                                    evaluator=self.evaluator,
+                                    dataset=self.dataset  # only used for Pykeen's models
+                                    )
         # (4) Start the training
         self.trained_model, form_of_labelling = self.trainer.start(dataset=self.dataset)
-        return self.end(start_time, form_of_labelling)
+        return self.end(form_of_labelling)
 
 
 class ContinuousExecute(Execute):
     """ A subclass of Execute Class for retraining
 
     (1) Loading & Preprocessing & Serializing input data.
     (2) Training & Validation & Testing
```

### Comparing `dicee-0.0.3/dicee/figures/deploy_qmult_family.png` & `dicee-0.0.4/dicee/figures/deploy_qmult_family.png`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/helper_classes.py` & `dicee-0.0.4/dicee/helper_classes.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/knowledge_graph.py` & `dicee-0.0.4/dicee/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/knowledge_graph_embeddings.py` & `dicee-0.0.4/dicee/knowledge_graph_embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
                     return deploy_head_entity_prediction(self, str_object, str_predicate, top_k)
                 elif self.is_seen(entity=str_subject) and self.is_seen(entity=str_object):
                     """ Relation Prediction """
                     return deploy_relation_prediction(self, str_subject, str_object, top_k)
                 else:
                     KeyError('Uncovered scenario')
             # If user simply select submit
-            return random_prediction(pre_trained_kge)
+            return random_prediction(self)
 
         gr.Interface(
             fn=predict,
             inputs=[gr.inputs.Textbox(lines=1, placeholder=None, label='Subject'),
                     gr.inputs.Textbox(lines=1, placeholder=None, label='Predicate'),
                     gr.inputs.Textbox(lines=1, placeholder=None, label='Object'), "checkbox"],
             outputs=[gr.outputs.Textbox(label='Input Triple'),
```

### Comparing `dicee-0.0.3/dicee/models/base_model.py` & `dicee-0.0.4/dicee/models/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         # Not quite sure about EstimatedSizeMB ?
         buffer_size = 0
         for buffer in self.buffers():
             buffer_size += buffer.nelement() * buffer.element_size()
         return {'EstimatedSizeMB': (num_params + buffer_size) / 1024 ** 2, 'NumParam': num_params}
 
     def init_params_with_sanity_checking(self):
-        assert self.args['model'] in ['FMult', 'FMult2', 'CMult', 'Keci', 'DistMult', 'ComplEx', 'QMult', 'OMult', 'ConvQ',
-                                      'ConvO', 'AConEx', 'ConEx', 'Shallom', 'TransE', 'Pyke', 'KeciBase', 'GFMult']
+        #assert self.args['model'] in ['FMult', 'FMult2', 'CMult', 'Keci', 'DistMult', 'ComplEx', 'QMult', 'OMult', 'ConvQ',
+        #                              'ConvO', 'AConEx', 'ConEx', 'Shallom', 'TransE', 'Pyke', 'KeciBase', 'GFMult']
         if self.args.get('weight_decay'):
             self.weight_decay = self.args['weight_decay']
         else:
             self.weight_decay = 0.0
         if self.args.get('embedding_dim'):
             self.embedding_dim = self.args['embedding_dim']
         else:
@@ -78,15 +78,15 @@
         else:
             self.input_dropout_rate = 0.0
         if self.args.get("hidden_dropout_rate"):
             self.hidden_dropout_rate = self.args['hidden_dropout_rate']
         else:
             self.hidden_dropout_rate = 0.0
 
-        if self.args['model'] in ['ConvQ', 'ConvO', 'ConEx', 'AConEx']:
+        if self.args['model'] in ['ConvQ', 'ConvO', 'ConEx', 'AConEx', 'AConvQ', 'AConvO']:
             if self.args.get("kernel_size"):
                 self.kernel_size = self.args['kernel_size']
             else:
                 self.kernel_size = 3
             if self.args.get("num_of_output_channels"):
                 self.num_of_output_channels = self.args['num_of_output_channels']
             else:
```

### Comparing `dicee-0.0.3/dicee/models/clifford.py` & `dicee-0.0.4/dicee/models/clifford.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/models/complex.py` & `dicee-0.0.4/dicee/models/complex.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/models/function_space.py` & `dicee-0.0.4/dicee/models/function_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def __init__(self, args):
         super().__init__(args)
         self.name = 'GFMult'
         self.entity_embeddings = torch.nn.Embedding(self.num_entities, self.embedding_dim)
         self.relation_embeddings = torch.nn.Embedding(self.num_relations, self.embedding_dim)
         self.param_init(self.entity_embeddings.weight.data), self.param_init(self.relation_embeddings.weight.data)
         self.k = int(np.sqrt(self.embedding_dim // 2))
-        self.num_sample = 50
+        self.num_sample = 250
         roots, weights = roots_legendre(self.num_sample)
         self.roots = torch.from_numpy(roots).repeat(self.k, 1).float()  # shape self.k by self.n
         self.weights = torch.from_numpy(weights).reshape(1, -1).float()  # shape 1 by self.n
 
     def compute_func(self, weights: torch.FloatTensor, x) -> torch.FloatTensor:
         n = len(weights)
         # Weights for two linear layers.
```

### Comparing `dicee-0.0.3/dicee/models/octonion.py` & `dicee-0.0.4/dicee/models/octonion.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     return x, e1, e2, e3, e4, e5, e6, e7
 
 
 class OMult(BaseKGE):
     def __init__(self, args):
         super().__init__(args)
-        self.name = 'QMult'
+        self.name = 'OMult'
         self.entity_embeddings = torch.nn.Embedding(self.num_entities, self.embedding_dim)
         self.relation_embeddings = torch.nn.Embedding(self.num_relations, self.embedding_dim)
         self.param_init(self.entity_embeddings.weight.data), self.param_init(self.relation_embeddings.weight.data)
 
     def forward_triples(self, x: torch.Tensor) -> torch.Tensor:
         # (1) Retrieve embeddings & Apply Dropout & Normalization.
         head_ent_emb, rel_ent_emb, tail_ent_emb = self.get_triple_representation(x)
@@ -253,7 +253,139 @@
         e3_score = torch.mm(conv_e3 * e3, emb_tail_e3)
         e4_score = torch.mm(conv_e4 * e4, emb_tail_e4)
         e5_score = torch.mm(conv_e5 * e5, emb_tail_e5)
         e6_score = torch.mm(conv_e6 * e6, emb_tail_e6)
         e7_score = torch.mm(conv_e7 * e7, emb_tail_e7)
         return e0_score + e1_score + e2_score + e3_score + e4_score + e5_score + e6_score + e7_score
 
+
+class AConvO(BaseKGE):
+    """ Additive Convolutional Octonion Knowledge Graph Embeddings """
+    def __init__(self, args: dict):
+        super().__init__(args=args)
+        self.name = 'AConvO'
+        self.entity_embeddings = torch.nn.Embedding(self.num_entities, self.embedding_dim)
+        self.relation_embeddings = torch.nn.Embedding(self.num_relations, self.embedding_dim)
+        self.param_init(self.entity_embeddings.weight.data), self.param_init(self.relation_embeddings.weight.data)
+        # Convolution
+        self.conv2d = torch.nn.Conv2d(in_channels=1, out_channels=self.num_of_output_channels,
+                                      kernel_size=(self.kernel_size, self.kernel_size), stride=1, padding=1, bias=True)
+        self.fc_num_input = self.embedding_dim * 2 * self.num_of_output_channels
+        self.fc1 = torch.nn.Linear(self.fc_num_input, self.embedding_dim)  # Hard compression.
+        self.bn_conv2d = torch.nn.BatchNorm2d(self.num_of_output_channels)
+        self.norm_fc1 = self.normalizer_class(self.embedding_dim)
+        self.feature_map_dropout = torch.nn.Dropout2d(self.feature_map_dropout_rate)
+
+    def residual_convolution(self, O_1, O_2):
+        emb_ent_e0, emb_ent_e1, emb_ent_e2, emb_ent_e3, emb_ent_e4, emb_ent_e5, emb_ent_e6, emb_ent_e7 = O_1
+        emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3, emb_rel_e4, emb_rel_e5, emb_rel_e6, emb_rel_e7 = O_2
+        x = torch.cat([emb_ent_e0.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e1.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e2.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e3.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e4.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e5.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e6.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_ent_e7.view(-1, 1, 1, self.embedding_dim // 8),  # entities
+                       emb_rel_e0.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e1.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e2.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e3.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e4.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e5.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e6.view(-1, 1, 1, self.embedding_dim // 8),
+                       emb_rel_e7.view(-1, 1, 1, self.embedding_dim // 8), ], 2)
+        x = torch.nn.functional.relu(self.bn_conv2d(self.conv2d(x)))
+        x = self.feature_map_dropout(x)
+        x = x.view(x.shape[0], -1)  # reshape for NN.
+        x = torch.nn.functional.relu(self.norm_fc1(self.fc1(x)))
+        return torch.chunk(x, 8, dim=1)
+
+    def forward_triples(self, x: torch.Tensor) -> torch.Tensor:
+
+        # (1) Retrieve embeddings & Apply Dropout & Normalization.
+        head_ent_emb, rel_ent_emb, tail_ent_emb = self.get_triple_representation(x)
+        # (2) Split (1) into real and imaginary parts.
+        emb_head_e0, emb_head_e1, emb_head_e2, emb_head_e3, emb_head_e4, emb_head_e5, emb_head_e6, emb_head_e7 = torch.hsplit(
+            head_ent_emb, 8)
+        emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3, emb_rel_e4, emb_rel_e5, emb_rel_e6, emb_rel_e7 = torch.hsplit(
+            rel_ent_emb,
+            8)
+        emb_tail_e0, emb_tail_e1, emb_tail_e2, emb_tail_e3, emb_tail_e4, emb_tail_e5, emb_tail_e6, emb_tail_e7 = torch.hsplit(
+            tail_ent_emb, 8)
+
+        # (2) Apply convolution operation on (1.1) and (1.2).
+        O_3 = self.residual_convolution(O_1=(emb_head_e0, emb_head_e1, emb_head_e2, emb_head_e3,
+                                             emb_head_e4, emb_head_e5, emb_head_e6, emb_head_e7),
+                                        O_2=(emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3,
+                                             emb_rel_e4, emb_rel_e5, emb_rel_e6, emb_rel_e7))
+        conv_e0, conv_e1, conv_e2, conv_e3, conv_e4, conv_e5, conv_e6, conv_e7 = O_3
+
+        # (3)
+        # (3.1) Apply quaternion multiplication.
+        e0, e1, e2, e3, e4, e5, e6, e7 = octonion_mul(
+            O_1=(emb_head_e0, emb_head_e1, emb_head_e2, emb_head_e3, emb_head_e4,
+                 emb_head_e5, emb_head_e6, emb_head_e7),
+            O_2=(emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3, emb_rel_e4,
+                 emb_rel_e5, emb_rel_e6, emb_rel_e7))
+        # (4)
+        # (4.4) Inner product
+        e0_score = (conv_e0 + e0 * emb_tail_e0).sum(dim=1)
+        e1_score = (conv_e1 + e1 * emb_tail_e1).sum(dim=1)
+        e2_score = (conv_e2 + e2 * emb_tail_e2).sum(dim=1)
+        e3_score = (conv_e3 + e3 * emb_tail_e3).sum(dim=1)
+        e4_score = (conv_e4 + e4 * emb_tail_e4).sum(dim=1)
+        e5_score = (conv_e5 + e5 * emb_tail_e5).sum(dim=1)
+        e6_score = (conv_e6 + e6 * emb_tail_e6).sum(dim=1)
+        e7_score = (conv_e7 + e7 * emb_tail_e7).sum(dim=1)
+        return e0_score + e1_score + e2_score + e3_score + e4_score + e5_score + e6_score + e7_score
+
+    def forward_k_vs_all(self, x: torch.Tensor):
+        """
+        Given a head entity and a relation (h,r), we compute scores for all entities.
+        [score(h,r,x)|x \in Entities] => [0.0,0.1,...,0.8], shape=> (1, |Entities|)
+        Given a batch of head entities and relations => shape (size of batch,| Entities|)
+        """
+
+        # (1) Retrieve embeddings & Apply Dropout & Normalization.
+        head_ent_emb, rel_ent_emb = self.get_head_relation_representation(x)
+        # (2) Split (1) into real and imaginary parts.
+        # (2) Split (1) into real and imaginary parts.
+        emb_head_e0, emb_head_e1, emb_head_e2, emb_head_e3, emb_head_e4, emb_head_e5, emb_head_e6, emb_head_e7 = torch.hsplit(
+            head_ent_emb, 8)
+        emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3, emb_rel_e4, emb_rel_e5, emb_rel_e6, emb_rel_e7 = torch.hsplit(
+            rel_ent_emb,
+            8)
+
+        # (2) Apply convolution operation on (1.1) and (1.2).
+        O_3 = self.residual_convolution(O_1=(emb_head_e0, emb_head_e1, emb_head_e2, emb_head_e3,
+                                             emb_head_e4, emb_head_e5, emb_head_e6, emb_head_e7),
+                                        O_2=(emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3,
+                                             emb_rel_e4, emb_rel_e5, emb_rel_e6, emb_rel_e7))
+        conv_e0, conv_e1, conv_e2, conv_e3, conv_e4, conv_e5, conv_e6, conv_e7 = O_3
+
+        # (3)
+        # (3.2) Apply quaternion multiplication on (1.1) and (3.1).
+        e0, e1, e2, e3, e4, e5, e6, e7 = octonion_mul(
+            O_1=(emb_head_e0, emb_head_e1, emb_head_e2, emb_head_e3, emb_head_e4,
+                 emb_head_e5, emb_head_e6, emb_head_e7),
+            O_2=(emb_rel_e0, emb_rel_e1, emb_rel_e2, emb_rel_e3, emb_rel_e4,
+                 emb_rel_e5, emb_rel_e6, emb_rel_e7))
+
+        emb_tail_e0, emb_tail_e1, emb_tail_e2, emb_tail_e3, emb_tail_e4, emb_tail_e5, emb_tail_e6, emb_tail_e7 = torch.hsplit(
+            self.entity_embeddings.weight, 8)
+        emb_tail_e0, emb_tail_e1, emb_tail_e2, emb_tail_e3, emb_tail_e4, emb_tail_e5, emb_tail_e6, emb_tail_e7 = emb_tail_e0.transpose(
+            1, 0), emb_tail_e1.transpose(1, 0), emb_tail_e2.transpose(1, 0), emb_tail_e3.transpose(1,
+                                                                                                   0), emb_tail_e4.transpose(
+            1, 0), emb_tail_e5.transpose(1, 0), emb_tail_e6.transpose(1, 0), emb_tail_e7.transpose(1, 0)
+
+        # (4)
+        # (4.4) Inner product
+        e0_score = torch.mm(conv_e0 + e0, emb_tail_e0)
+        e1_score = torch.mm(conv_e1 + e1, emb_tail_e1)
+        e2_score = torch.mm(conv_e2 + e2, emb_tail_e2)
+        e3_score = torch.mm(conv_e3 + e3, emb_tail_e3)
+        e4_score = torch.mm(conv_e4 + e4, emb_tail_e4)
+        e5_score = torch.mm(conv_e5 + e5, emb_tail_e5)
+        e6_score = torch.mm(conv_e6 + e6, emb_tail_e6)
+        e7_score = torch.mm(conv_e7 + e7, emb_tail_e7)
+        return e0_score + e1_score + e2_score + e3_score + e4_score + e5_score + e6_score + e7_score
```

### Comparing `dicee-0.0.3/dicee/models/quaternion.py` & `dicee-0.0.4/dicee/models/quaternion.py`

 * *Files 21% similar despite different names*

```diff
@@ -114,16 +114,14 @@
         real_score = torch.bmm(r_val, emb_tail_real)
         i_score = torch.bmm(i_val, emb_tail_i)
         j_score = torch.bmm(j_val, emb_tail_j)
         k_score = torch.bmm(k_val, emb_tail_k)
 
         return (real_score + i_score + j_score + k_score).squeeze(1)
 
-
-
 class ConvQ(BaseKGE):
     """ Convolutional Quaternion Knowledge Graph Embeddings
 
     """
 
     def __init__(self, args):
         super().__init__(args)
@@ -221,7 +219,111 @@
         # (4.1) Hadamard product of (2) with (3) and inner product with tails
         real_score = torch.mm(conv_real * r_val, emb_tail_real)
         i_score = torch.mm(conv_imag_i * i_val, emb_tail_i)
         j_score = torch.mm(conv_imag_j * j_val, emb_tail_j)
         k_score = torch.mm(conv_imag_k * k_val, emb_tail_k)
 
         return real_score + i_score + j_score + k_score
+
+class AConvQ(BaseKGE):
+    """ Additive Convolutional Quaternion Knowledge Graph Embeddings """
+
+    def __init__(self, args):
+        super().__init__(args)
+        self.name = 'AConvQ'
+        self.entity_embeddings = torch.nn.Embedding(self.num_entities, self.embedding_dim)
+        self.relation_embeddings = torch.nn.Embedding(self.num_relations, self.embedding_dim)
+        self.param_init(self.entity_embeddings.weight.data), self.param_init(self.relation_embeddings.weight.data)
+        # Convolution
+        self.conv2d = torch.nn.Conv2d(in_channels=1, out_channels=self.num_of_output_channels,
+                                      kernel_size=(self.kernel_size, self.kernel_size), stride=1, padding=1, bias=True)
+
+        self.fc_num_input = self.embedding_dim * 2 * self.num_of_output_channels  # 8 because of 8 real values in 2 quaternions
+        self.fc1 = torch.nn.Linear(self.fc_num_input, self.embedding_dim)  # Hard compression.
+
+        self.bn_conv1 = torch.nn.BatchNorm2d(self.num_of_output_channels)
+        self.bn_conv2 = self.normalizer_class(self.embedding_dim)
+        self.feature_map_dropout = torch.nn.Dropout2d(self.feature_map_dropout_rate)
+
+    def residual_convolution(self, Q_1, Q_2):
+        emb_ent_real, emb_ent_imag_i, emb_ent_imag_j, emb_ent_imag_k = Q_1
+        emb_rel_real, emb_rel_imag_i, emb_rel_imag_j, emb_rel_imag_k = Q_2
+        x = torch.cat([emb_ent_real.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_ent_imag_i.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_ent_imag_j.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_ent_imag_k.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_rel_real.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_rel_imag_i.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_rel_imag_j.view(-1, 1, 1, self.embedding_dim // 4),
+                       emb_rel_imag_k.view(-1, 1, 1, self.embedding_dim // 4)], 2)
+
+        # n, c_in, h_in, w_in x.shape before conv. h_in=8, w_in embeddings
+        x = self.conv2d(x)
+        # n, c_out, h_out, w_out x.shape after conv.
+        x = self.bn_conv1(x)
+        x = torch.nn.functional.relu(x)
+        x = self.feature_map_dropout(x)
+        x = x.view(x.shape[0], -1)  # reshape for NN.
+        x = torch.nn.functional.relu(self.bn_conv2(self.fc1(x)))
+        return torch.chunk(x, 4, dim=1)
+
+    def forward_triples(self, indexed_triple: torch.Tensor) -> torch.Tensor:
+        # (1) Retrieve embeddings & Apply Dropout & Normalization.
+        head_ent_emb, rel_ent_emb, tail_ent_emb = self.get_triple_representation(indexed_triple)
+        # (2) Split (1) into real and imaginary parts.
+        emb_head_real, emb_head_i, emb_head_j, emb_head_k = torch.hsplit(head_ent_emb, 4)
+        emb_rel_real, emb_rel_i, emb_rel_j, emb_rel_k = torch.hsplit(rel_ent_emb, 4)
+        emb_tail_real, emb_tail_i, emb_tail_j, emb_tail_k = torch.hsplit(tail_ent_emb, 4)
+
+        # (2) Apply convolution operation on (1.1) and (1.2).
+        Q_3 = self.residual_convolution(Q_1=(emb_head_real, emb_head_i, emb_head_j, emb_head_k),
+                                        Q_2=(emb_rel_real, emb_rel_i, emb_rel_j, emb_rel_k))
+        conv_real, conv_imag_i, conv_imag_j, conv_imag_k = Q_3
+        # (3)
+        # (3.1) Apply quaternion multiplication on (1.1) and (3.1).
+        r_val, i_val, j_val, k_val = quaternion_mul(
+            Q_1=(emb_head_real, emb_head_i, emb_head_j, emb_head_k),
+            Q_2=(emb_rel_real, emb_rel_i, emb_rel_j, emb_rel_k))
+        # (4)
+        # (4.1) Hadamard product of (2) with (3) and inner product with tails
+        real_score = torch.sum(conv_real + r_val * emb_tail_real, dim=1)
+        i_score = torch.sum(conv_imag_i + i_val * emb_tail_i, dim=1)
+        j_score = torch.sum(conv_imag_j + j_val * emb_tail_j, dim=1)
+        k_score = torch.sum(conv_imag_k + k_val * emb_tail_k, dim=1)
+        return real_score + i_score + j_score + k_score
+
+    def forward_k_vs_all(self, x: torch.Tensor):
+        """
+        Given a head entity and a relation (h,r), we compute scores for all entities.
+        [score(h,r,x)|x \in Entities] => [0.0,0.1,...,0.8], shape=> (1, |Entities|)
+        Given a batch of head entities and relations => shape (size of batch,| Entities|)
+        """
+
+        # (1) Retrieve embeddings & Apply Dropout & Normalization.
+        head_ent_emb, rel_ent_emb = self.get_head_relation_representation(x)
+        # (2) Split (1) into real and imaginary parts.
+        emb_head_real, emb_head_i, emb_head_j, emb_head_k = torch.hsplit(head_ent_emb, 4)
+        emb_rel_real, emb_rel_i, emb_rel_j, emb_rel_k = torch.hsplit(rel_ent_emb, 4)
+
+        # (2) Apply convolution operation on (1.1) and (1.2).
+        Q_3 = self.residual_convolution(Q_1=(emb_head_real, emb_head_i, emb_head_j, emb_head_k),
+                                        Q_2=(emb_rel_real, emb_rel_i, emb_rel_j, emb_rel_k))
+        conv_real, conv_imag_i, conv_imag_j, conv_imag_k = Q_3
+
+        # (3)
+        # (3.1) Apply quaternion multiplication.
+        r_val, i_val, j_val, k_val = quaternion_mul(Q_1=(emb_head_real, emb_head_i, emb_head_j, emb_head_k),
+                                                    Q_2=(emb_rel_real, emb_rel_i, emb_rel_j, emb_rel_k))
+        # Prepare all entity embeddings.
+        emb_tail_real, emb_tail_i, emb_tail_j, emb_tail_k = torch.hsplit(self.entity_embeddings.weight, 4)
+        emb_tail_real, emb_tail_i, emb_tail_j, emb_tail_k = emb_tail_real.transpose(1, 0), emb_tail_i.transpose(1,
+                                                                                                                0), emb_tail_j.transpose(
+            1, 0), emb_tail_k.transpose(1, 0)
+
+        # (4)
+        # (4.1) Hadamard product of (2) with (3) and inner product with tails
+        real_score = torch.mm(conv_real + r_val, emb_tail_real)
+        i_score = torch.mm(conv_imag_i + i_val, emb_tail_i)
+        j_score = torch.mm(conv_imag_j + j_val, emb_tail_j)
+        k_score = torch.mm(conv_imag_k + k_val, emb_tail_k)
+
+        return real_score + i_score + j_score + k_score
```

### Comparing `dicee-0.0.3/dicee/models/real.py` & `dicee-0.0.4/dicee/models/real.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/models/static_funcs.py` & `dicee-0.0.4/dicee/models/static_funcs.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/read_preprocess_save_load_kg/preprocess.py` & `dicee-0.0.4/dicee/read_preprocess_save_load_kg/preprocess.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/read_preprocess_save_load_kg/read_from_disk.py` & `dicee-0.0.4/dicee/read_preprocess_save_load_kg/read_from_disk.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/read_preprocess_save_load_kg/save_load_disk.py` & `dicee-0.0.4/dicee/read_preprocess_save_load_kg/save_load_disk.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/read_preprocess_save_load_kg/util.py` & `dicee-0.0.4/dicee/read_preprocess_save_load_kg/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,57 +24,14 @@
             f'Took {total_time:.4f} seconds | Current Memory Usage {psutil.Process(os.getpid()).memory_info().rss / 1000000: .5} in MB')
         return result
 
     return timeit_wrapper
 
 
 @timeit
-def read_with_modin(data_path, read_only_few: int = None, sample_triples_ratio: float = None):
-    print(f'*** Reading {data_path} with Modin ***')
-
-    import modin.pandas as pd
-    if data_path[-3:] in ['txt', 'csv']:
-        print('Reading with modin.read_csv with sep ** s+ ** ...')
-        df = pd.read_csv(data_path,
-                         sep='\s+',
-                         header=None,
-                         usecols=[0, 1, 2],
-                         names=['subject', 'relation', 'object'],
-                         dtype=str)
-    else:
-        df = pd.read_parquet(data_path, engine='pyarrow')
-
-    # df <class 'modin.pandas.dataframe.DataFrame'>
-    # return pandas DataFrame
-    # (2)a Read only few if it is asked.
-    if isinstance(read_only_few, int):
-        if read_only_few > 0:
-            print(f'Reading only few input data {read_only_few}...')
-            df = df.head(read_only_few)
-            print('Done !\n')
-    # (3) Read only sample
-    if sample_triples_ratio:
-        print(f'Subsampling {sample_triples_ratio} of input data...')
-        df = df.sample(frac=sample_triples_ratio)
-        print('Done !\n')
-    if sum(df.head()["subject"].str.startswith('<')) + sum(df.head()["relation"].str.startswith('<')) > 2:
-        # (4) Drop Rows/triples with double or boolean: Example preprocessing
-        # Drop of object does not start with **<**.
-        # Specifying na to be False instead of NaN.
-        print('Removing triples with literal values...')
-        df = df[df["object"].str.startswith('<', na=False)]
-        print('Done !\n')
-        # (5) Remove **<** and **>**
-        print('Removing brackets **<** and **>**...')
-        df = df.apply(lambda x: x.str.removeprefix("<").str.removesuffix(">"), axis=1)
-        print('Done !\n')
-    return df._to_pandas()
-
-
-@timeit
 def read_with_polars(data_path, read_only_few: int = None, sample_triples_ratio: float = None) -> polars.DataFrame:
     """ Load and Preprocess via Polars """
     print(f'*** Reading {data_path} with Polars ***')
     # (1) Load the data
     if data_path[-3:] in ['txt', 'csv']:
         print('Reading with polars.read_csv with sep **t** ...')
         df = polars.read_csv(data_path,
@@ -105,30 +62,31 @@
         df = df.filter(polars.col("object").str.starts_with('<'))
     return df
 
 
 @timeit
 def read_with_pandas(data_path, read_only_few: int = None, sample_triples_ratio: float = None):
     print(f'*** Reading {data_path} with Pandas ***')
-    if data_path[-3:] in ['txt', 'csv']:
+    if data_path[-3:] in ['txt', 'csv','zst']:
         print('Reading with pandas.read_csv with sep ** s+ ** ...')
         df = pd.read_csv(data_path,
                          sep="\s+",
                          header=None,
+                         nrows=None if read_only_few is None else read_only_few,
                          usecols=[0, 1, 2],
                          names=['subject', 'relation', 'object'],
                          dtype=str)
     else:
         df = pd.read_parquet(data_path, engine='pyarrow')
-    # (2)a Read only few if it is asked.
-    if isinstance(read_only_few, int):
-        if read_only_few > 0:
-            print(f'Reading only few input data {read_only_few}...')
-            df = df.head(read_only_few)
-            print('Done !\n')
+        # (2)a Read only few if it is asked.
+        if isinstance(read_only_few, int):
+            if read_only_few > 0:
+                print(f'Reading only few input data {read_only_few}...')
+                df = df.head(read_only_few)
+                print('Done !\n')
     # (3) Read only sample
     if sample_triples_ratio:
         print(f'Subsampling {sample_triples_ratio} of input data...')
         df = df.sample(frac=sample_triples_ratio)
         print('Done !\n')
     if sum(df.head()["subject"].str.startswith('<')) + sum(df.head()["relation"].str.startswith('<')) > 2:
         # (4) Drop Rows/triples with double or boolean: Example preprocessing
```

### Comparing `dicee-0.0.3/dicee/sanity_checkers.py` & `dicee-0.0.4/dicee/sanity_checkers.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/static_funcs.py` & `dicee-0.0.4/dicee/static_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-import os
 import numpy as np
+import pykeen.models
 import torch
 import datetime
 from .types import Tuple
-from .models import Shallom, ConEx, AConEx, QMult, OMult, ConvQ, ConvO, ComplEx, DistMult, TransE, Keci, CMult, KeciBase, Pyke, FMult, FMult2, GFMult
+from .models import *
+from .models.pykeen_models import PykeenKGE
 from .models.base_model import BaseKGE
 import time
 import pandas as pd
 import json
 import glob
 import pandas
 import polars
 import functools
-import pickle
 import os
 import psutil
+import torch
+import datetime
+from .types import Tuple
+from .models.base_model import BaseKGE
+import time
+import json
+import glob
+import pandas
+import polars
+import pickle
+import pytorch_lightning as pl
+from pykeen.datasets.base import EagerDataset
+from pykeen.triples.triples_factory import TriplesFactory
 
 
 def timeit(func):
     @functools.wraps(func)
     def timeit_wrapper(*args, **kwargs):
         start_time = time.perf_counter()
         result = func(*args, **kwargs)
@@ -31,21 +44,21 @@
     return timeit_wrapper
 
 
 def save_pickle(*, data: object, file_path=str):
     pickle.dump(data, open(file_path, "wb"))
 
 
-def load_pickle(*, file_path=str):
+def load_pickle(file_path=str):
     with open(file_path, 'rb') as f:
         return pickle.load(f)
 
 
 # @TODO: Could these funcs can be merged?
-def select_model(args: dict, is_continual_training: bool = None, storage_path: str = None):
+def select_model(args: dict, is_continual_training: bool = None, storage_path: str = None, dataset=None):
     isinstance(args, dict)
     assert len(args) > 0
     assert isinstance(is_continual_training, bool)
     assert isinstance(storage_path, str)
     if is_continual_training:
         print('Loading pre-trained model...')
         model, _ = intialize_model(args)
@@ -55,15 +68,15 @@
             for parameter in model.parameters():
                 parameter.requires_grad = True
             model.train()
         except FileNotFoundError:
             print(f"{storage_path}/model.pt is not found. The model will be trained with random weights")
         return model, _
     else:
-        return intialize_model(args)
+        return intialize_model(args, dataset)
 
 
 def load_model(path_of_experiment_folder, model_name='model.pt') -> Tuple[object, dict, dict]:
     """ Load weights and initialize pytorch module from namespace arguments"""
     print(f'Loading model {model_name}...', end=' ')
     start_time = time.time()
     # (1) Load weights..
@@ -173,22 +186,26 @@
         # print(f'Setting int32,\t {np.iinfo(np.int32).max}')
         train_set = train_set.astype(np.int32)
     else:
         raise TypeError('Int64?')
     return train_set
 
 
-def save_checkpoint_model(trainer, model, path: str) -> None:
+def save_checkpoint_model(model, path: str) -> None:
     """ Store Pytorch model into disk"""
-    try:
-        torch.save(model.state_dict(), path)
-    except ReferenceError as e:
-        print(e)
-        print(model.name)
-        print('Could not save the model correctly')
+    if isinstance(model, BaseKGE):
+        try:
+            torch.save(model.state_dict(), path)
+        except ReferenceError as e:
+            print(e)
+            print(model.name)
+            print('Could not save the model correctly')
+    else:
+        # Pykeen
+        torch.save(model.model.state_dict(), path)
 
 
 def store(trainer,
           trained_model, model_name: str = 'model', full_storage_path: str = None,
           dataset=None, save_as_csv=False) -> None:
     """
     Store trained_model model and save embeddings into csv file.
@@ -201,16 +218,15 @@
     :return:
     """
     assert full_storage_path is not None
     assert isinstance(model_name, str)
     assert len(model_name) > 1
 
     # (1) Save pytorch model in trained_model .
-    save_checkpoint_model(trainer=trainer,
-                          model=trained_model, path=full_storage_path + f'/{model_name}.pt')
+    save_checkpoint_model(model=trained_model, path=full_storage_path + f'/{model_name}.pt')
     if save_as_csv:
         entity_emb, relation_ebm = trained_model.get_embeddings()
         entity_to_idx = pickle.load(open(full_storage_path + '/entity_to_idx.p', 'rb'))
         entity_str = entity_to_idx.keys()
         # Ensure that the ordering is correct.
         assert list(range(0, len(entity_str))) == list(entity_to_idx.values())
         save_embeddings(entity_emb.numpy(), indexes=entity_str,
@@ -270,19 +286,39 @@
              backend=args.backend)
     print(f'Preprocessing took: {time.time() - start_time:.3f} seconds')
     # (2) Share some info about data for easy access.
     print(kg.description_of_input)
     return kg
 
 
-def intialize_model(args: dict) -> Tuple[object, str]:
+def get_pykeen_model(model_name: str, args, dataset):
+    actual_name = model_name.split("_")[1]
+    if dataset is None:
+        # (1) Load a pretrained Pykeen Model
+        return PykeenKGE(model_name=actual_name,
+                         dataset=EagerDataset(
+                             training=TriplesFactory(load_numpy(args['full_storage_path']+'/train_set.npy'), load_pickle(file_path=args['full_storage_path']+'/entity_to_idx.p'), load_pickle(file_path=args['full_storage_path']+'/relation_to_idx.p')),
+                             testing=None), args=args)
+    elif args['scoring_technique'] in ['KvsAll', "NegSample"]:
+        return PykeenKGE(model_name=actual_name,
+                         dataset=EagerDataset(
+                             training=TriplesFactory(dataset.train_set, dataset.entity_to_idx, dataset.relation_to_idx),
+                             testing=None), args=args)
+    else:
+        raise NotImplementedError("Incorrect scoring technique")
+
+
+def intialize_model(args: dict, dataset=None) -> Tuple[object, str]:
     # @TODO: Apply construct_krone as callback? or use KronE_QMult as a prefix.
     # @TODO: Remove form_of_labelling
     model_name = args['model']
-    if model_name == 'Shallom':
+    if "pykeen" in model_name.lower():
+        model = get_pykeen_model(model_name, args, dataset)
+        form_of_labelling = "EntityPrediction"
+    elif model_name == 'Shallom':
         model = Shallom(args=args)
         form_of_labelling = 'RelationPrediction'
     elif model_name == 'ConEx':
         model = ConEx(args=args)
         form_of_labelling = 'EntityPrediction'
     elif model_name == 'AConEx':
         model = AConEx(args=args)
@@ -292,17 +328,23 @@
         form_of_labelling = 'EntityPrediction'
     elif model_name == 'OMult':
         model = OMult(args=args)
         form_of_labelling = 'EntityPrediction'
     elif model_name == 'ConvQ':
         model = ConvQ(args=args)
         form_of_labelling = 'EntityPrediction'
+    elif model_name == 'AConvQ':
+        model = AConvQ(args=args)
+        form_of_labelling = 'EntityPrediction'
     elif model_name == 'ConvO':
         model = ConvO(args=args)
         form_of_labelling = 'EntityPrediction'
+    elif model_name == 'AConvO':
+        model = AConvO(args=args)
+        form_of_labelling = 'EntityPrediction'
     elif model_name == 'ComplEx':
         model = ComplEx(args=args)
         form_of_labelling = 'EntityPrediction'
     elif model_name == 'DistMult':
         model = DistMult(args=args)
         form_of_labelling = 'EntityPrediction'
     elif model_name == 'TransE':
```

### Comparing `dicee-0.0.3/dicee/static_preprocess_funcs.py` & `dicee-0.0.4/dicee/static_preprocess_funcs.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/trainer/dice_trainer.py` & `dicee-0.0.4/dicee/trainer/dice_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         else:
             print('Initializing TorchTrainer CPU Trainer', end='\t')
             return TorchTrainer(args, callbacks=callbacks)
     elif args.trainer == 'PL':
         print('Initializing Pytorch-lightning Trainer', end='\t')
         # Pytest with PL problem https://github.com/pytest-dev/pytest/discussions/7995
         return pl.Trainer.from_argparse_args(args,
+                                             callbacks=callbacks,
                                              strategy=DDPStrategy(find_unused_parameters=False))
     else:
         print('Initialize TorchTrainer CPU Trainer', end='\t')
         return TorchTrainer(args, callbacks=callbacks)
 
 
 def get_callbacks(args):
@@ -105,23 +106,24 @@
     evaluator:
 
     Returns
     -------
     report:dict
     """
 
-    def __init__(self, args, is_continual_training, storage_path, evaluator=None):
+    def __init__(self, args, is_continual_training, storage_path, evaluator=None,dataset=None):
         self.report = dict()
         self.args = args
         self.trainer = None
         self.is_continual_training = is_continual_training
         self.storage_path = storage_path
         # Required for CV.
         self.evaluator = evaluator
         self.form_of_labelling=None
+        self.dataset=dataset
         print(
             f'# of CPUs:{os.cpu_count()} | # of GPUs:{torch.cuda.device_count()} | # of CPUs for dataloader:{self.args.num_core}')
 
         for i in range(torch.cuda.device_count()):
             print(torch.cuda.get_device_name(i))
 
     def continual_start(self):
@@ -156,28 +158,27 @@
     def initialize_trainer(self, callbacks: List, plugins: List) -> pl.Trainer:
         """ Initialize Trainer from input arguments """
         return initialize_trainer(self.args, callbacks)
 
     @timeit
     def initialize_or_load_model(self):
         print('Initializing Model...', end='\t')
-        model, form_of_labelling = select_model(vars(self.args), self.is_continual_training, self.storage_path)
+        model, form_of_labelling = select_model(vars(self.args), self.is_continual_training, self.storage_path,self.dataset)
         self.report['form_of_labelling'] = form_of_labelling
         assert form_of_labelling in ['EntityPrediction', 'RelationPrediction']
         return model, form_of_labelling
 
     @timeit
     def initialize_dataloader(self, dataset: torch.utils.data.Dataset) -> torch.utils.data.DataLoader:
         print('Initializing Dataloader...', end='\t')
         # https://pytorch.org/docs/stable/data.html#multi-process-data-loading
         # https://github.com/pytorch/pytorch/issues/13246#issuecomment-905703662
         return torch.utils.data.DataLoader(dataset=dataset, batch_size=self.args.batch_size,
                                            shuffle=True, collate_fn=dataset.collate_fn,
                                            num_workers=self.args.num_core, persistent_workers=False)
-
     @timeit
     def initialize_dataset(self, dataset, form_of_labelling) -> torch.utils.data.Dataset:
         print('Initializing Dataset...', end='\t')
         train_dataset = construct_dataset(train_set=dataset.train_set,
                                           valid_set=dataset.valid_set,
                                           test_set=dataset.test_set,
                                           entity_to_idx=dataset.entity_to_idx,
@@ -203,15 +204,14 @@
         else:
             self.trainer: Union[TorchTrainer, TorchDDPTrainer, pl.Trainer]
             self.trainer = self.initialize_trainer(callbacks=get_callbacks(self.args), plugins=[])
             model, form_of_labelling = self.initialize_or_load_model()
             self.trainer.evaluator=self.evaluator
             self.trainer.dataset = dataset
             self.trainer.form_of_labelling = form_of_labelling
-
             self.trainer.fit(model, train_dataloaders=self.initialize_dataloader(self.initialize_dataset(dataset, form_of_labelling)))
             return model, form_of_labelling
 
     def k_fold_cross_validation(self, dataset) -> Tuple[BaseKGE, str]:
         """
         Perform K-fold Cross-Validation
```

### Comparing `dicee-0.0.3/dicee/trainer/torch_trainer.py` & `dicee-0.0.4/dicee/trainer/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee/trainer/torch_trainer_ddp.py` & `dicee-0.0.4/dicee/trainer/torch_trainer_ddp.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/dicee.egg-info/PKG-INFO` & `dicee-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: dicee
-Version: 0.0.3
-Summary: Dice embedding is an hardware-agnostic framework for large-scale knowledge graph embedding applications
-Home-page: https://github.com/dice-group/dice-embeddings
-Author: Caglar Demir
-Author-email: caglardemir8@gmail.com
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DICE Embeddings: Hardware-agnostic Framework for Large-scale Knowledge Graph Embeddings
 
 Knowledge graph embedding research has mainly focused on learning continuous representations of knowledge graphs towards the link prediction problem. 
 Recently developed frameworks can be effectively applied in a wide range of research-related applications.
 Yet, using these frameworks in real-world applications becomes more challenging as the size of the knowledge graph grows.
 
 We developed the DICE Embeddings framework (dicee) to compute embeddings for large-scale knowledge graphs in a hardware-agnostic manner.
@@ -35,33 +22,37 @@
 Users can choose the trainer class (e.g., DDP by Pytorch) to train large knowledge graph embedding models with billions of parameters.
 PytorchLightning allows us to use state-of-the-art model parallelism techniques (e.g. Fully Sharded Training, FairScale, or DeepSpeed)
 without extra effort.
 With our framework, practitioners can directly use PytorchLightning for model parallelism to train gigantic embedding models.
 
 **Why [Hugging-face Gradio](https://huggingface.co/gradio)?**
 Deploy a pre-trained embedding model without writing a single line of code.
+# Installation
+<details><summary> Details </summary>
 
-
-## Installation
-```
+``` 
 pip install dicee
 ```
+
 or
+
 ```
 git clone https://github.com/dice-group/dice-embeddings.git
 conda create -n dice python=3.10 --no-default-packages && conda activate dice
 pip3 install "pandas>=1.5.1"
 pip3 install "torch>=2.0.0"
 pip3 install "polars>=0.16.14"
 pip3 install "scikit-learn>=1.2.2"
 pip3 install "pyarrow>=11.0.0"
 pip3 install "pytest>=7.2.2"
 pip3 install "gradio>=3.23.0"
 pip3 install "psutil>=5.9.4"
 pip3 install "pytorch-lightning==1.6.4"
+pip3 install "pykeen==1.10.1"
+pip3 install "zstandard>=0.21.0"
 ```
 To test the Installation
 ```
 wget https://hobbitdata.informatik.uni-leipzig.de/KG/KGs.zip
 unzip KGs.zip
 pytest -p no:warnings -x # it takes circa 15 minutes
 pytest -p no:warnings --lf # run only the last failed test
@@ -69,35 +60,42 @@
 ```
 To see the software architecture, execute the following command
 ```
 pyreverse dicee/ && dot -Tpng -x classes.dot -o dice_software.png && eog dice_software.png
 # or
 pyreverse dicee/trainer && dot -Tpng -x classes.dot -o trainer.png && eog trainer.png
 ```
-## Applications
-### Description Logic Concept Learning (soon)
-```python
-from dicee import KGE
-# (1) Load a pretrained KGE model on KGs/Family
-pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
-pretrained_model.learn_concepts(pos={''},neg={''},topk=1)
-```
-### Conjunctive Query/Question Answering
+</details>
+
+# Knowledge Graph Embedding Models
+<details> <summary> Details</summary>
+
+1. TransE, DistMult, ComplEx, ConEx, QMult, OMult, ConvO, ConvQ, Keci
+2. All 44 models available in https://github.com/pykeen/pykeen#models
+
+> For more, please refer to `examples`.
+</details>
+
+# How to Train
+<details> <summary> Details</summary>
+
+> Please refer to `examples`.
+</details>
+
+
+# How to Deploy
 ```python
 from dicee import KGE
-# (1) Load a pretrained KGE model on KGs/Family
-pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
-# (2) Answer the following conjunctive query question: To whom a sibling of F9M167 is married to?
-# (3) Decompose (2) into two query
-# (3.1) Who is a sibling of F9M167? => {F9F141,F9M157}
-# (3.2) To whom a results of (3.1) is married to ? {F9M142, F9F158}
-pretrained_model.predict_conjunctive_query(entity='<http://www.benchmark.org/family#F9M167>',
-                                          relations=['<http://www.benchmark.org/family#hasSibling>',
-                                                     '<http://www.benchmark.org/family#married>'], topk=1)
+KGE(path='...').deploy(share=True,top_k=10)
 ```
+<details> <summary> To see the interface of the webservice</summary>
+<img src="dicee/lp.png" alt="Italian Trulli">
+</details>
+
+## Downstream Applications
 ### Triple Classification
 #### Using pre-trained ConEx on DBpedia 03-2022
 ```bash
 # To download a pretrained ConEx
 mkdir ConEx && cd ConEx && wget -r -nd -np https://hobbitdata.informatik.uni-leipzig.de/KGE/DBpedia/ConEx/ && cd ..
 ```
 ```python
@@ -127,25 +125,38 @@
 ```
 ### Finding Missing Triples
 ```python
 from dicee import KGE
 pre_trained_kge = KGE(path='ConEx')
 missing_triples = pre_trained_kge.find_missing_triples(confidence=0.95, entities=[''], relations=[''])
 ```
+### Complex Query Answering
+The beam search technique proposed in [Complex Query Answering with Neural Link Predictors](https://arxiv.org/abs/2011.03459)
+```python
+from dicee import KGE
+# (1) Load a pretrained KGE model on KGs/Family
+pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
+# (2) Query: ?P : \exist Married(P,E) \land hasSibling(E, F9M167) (To whom a sibling of F9M167 is married to?   
+# (3) Decompose (2) into two query
+# (3.1) Who is a sibling of F9M167? => hasSibling(E, F9M167) => {F9F141,F9M157}
+# (3.2) To whom a results of (3.1) is married to ? {F9M142, F9F158}
+pretrained_model.predict_conjunctive_query(entity='<http://www.benchmark.org/family#F9M167>',
+                                          relations=['<http://www.benchmark.org/family#hasSibling>',
+                                                     '<http://www.benchmark.org/family#married>'], topk=1)
+```
 
-## How to Train a KGE model 
-> How to use the framework:`examples`.
-
-## How to Deploy
-Any pretrained model can be deployed with an ease. By setting ```share=True```, anyone on the internet can use a pretrained model.
+### Description Logic Concept Learning (soon)
 ```python
 from dicee import KGE
-KGE(path='...').deploy(share=True,top_k=10)
+# (1) Load a pretrained KGE model on KGs/Family
+pretrained_model = KGE(path='Experiments/2022-12-08 11:46:33.654677')
+pretrained_model.learn_concepts(pos={''},neg={''},topk=1)
 ```
-![alt text](dicee/figures/deploy_qmult_family.png)
+
+
 ## Pre-trained Models
 Please contact:  ```caglar.demir@upb.de ``` or ```caglardemir8@gmail.com ``` , if you lack hardware resources to obtain embeddings of a specific knowledge Graph.
 - [DBpedia version: 06-2022 Embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/DBpediaQMultEmbeddings_03_07):
   - Models: ConEx, QMult
 - [YAGO3-10 ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/YAGO3-10.zip)
 - [FB15K-237 ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/FB15K-237.zip)
 - [WN18RR ConEx embeddings](https://hobbitdata.informatik.uni-leipzig.de/KGE/conex/WN18RR.zip)
@@ -161,19 +172,22 @@
 @article{demir2022hardware,
   title={Hardware-agnostic computation for large-scale knowledge graph embeddings},
   author={Demir, Caglar and Ngomo, Axel-Cyrille Ngonga},
   journal={Software Impacts},
   year={2022},
   publisher={Elsevier}
 }
+# Keci
+Accepted at ECML. Stay tuned for the manuscript!
 # KronE
-@article{demir2022kronecker,
-  title={Kronecker Decomposition for Knowledge Graph Embeddings},
-  author={Demir, Caglar and Lienen, Julian and Ngomo, Axel-Cyrille Ngonga},
-  journal={arXiv preprint arXiv:2205.06560},
+@inproceedings{demir2022kronecker,
+  title={Kronecker decomposition for knowledge graph embeddings},
+  author={Demir, Caglar and Lienen, Julian and Ngonga Ngomo, Axel-Cyrille},
+  booktitle={Proceedings of the 33rd ACM Conference on Hypertext and Social Media},
+  pages={1--10},
   year={2022}
 }
 # QMult, OMult, ConvQ, ConvO
 @InProceedings{pmlr-v157-demir21a,
   title = 	 {Convolutional Hypercomplex Embeddings for Link Prediction},
   author =       {Demir, Caglar and Moussallem, Diego and Heindorf, Stefan and Ngonga Ngomo, Axel-Cyrille},
   booktitle = 	 {Proceedings of The 13th Asian Conference on Machine Learning},
```

### Comparing `dicee-0.0.3/dicee.egg-info/SOURCES.txt` & `dicee-0.0.4/dicee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Kronecker_classes.py
 LICENSE
 MANIFEST.in
 README.md
 analyse_experiments.py
 continual_training.py
 dl_learning.py
+dummy.py
 environment.yml
 example_class_combine_kge.py
 gpt.py
 large_file_preprocessing.txt
 main.py
 meta_heuristic.py
 out_of_sample.py
@@ -21,14 +22,15 @@
 dicee/config.py
 dicee/dataset_classes.py
 dicee/evaluator.py
 dicee/executer.py
 dicee/helper_classes.py
 dicee/knowledge_graph.py
 dicee/knowledge_graph_embeddings.py
+dicee/lp.png
 dicee/sanity_checkers.py
 dicee/static_funcs.py
 dicee/static_funcs_training.py
 dicee/static_preprocess_funcs.py
 dicee/types.py
 dicee.egg-info/PKG-INFO
 dicee.egg-info/SOURCES.txt
@@ -38,14 +40,15 @@
 dicee/figures/deploy_qmult_family.png
 dicee/models/__init__.py
 dicee/models/base_model.py
 dicee/models/clifford.py
 dicee/models/complex.py
 dicee/models/function_space.py
 dicee/models/octonion.py
+dicee/models/pykeen_models.py
 dicee/models/quaternion.py
 dicee/models/real.py
 dicee/models/static_funcs.py
 dicee/read_preprocess_save_load_kg/__init__.py
 dicee/read_preprocess_save_load_kg/preprocess.py
 dicee/read_preprocess_save_load_kg/read_from_disk.py
 dicee/read_preprocess_save_load_kg/save_load_disk.py
@@ -75,14 +78,15 @@
 tests/test_k_fold_cv_1_vs_all.py
 tests/test_k_fold_cv_k_vs_all.py
 tests/test_k_fold_cv_neg_sample.py
 tests/test_kvssample.py
 tests/test_large_kg.py
 tests/test_online_learning.py
 tests/test_pickle.py
+tests/test_pykeen.py
 tests/test_read_few_only.py
 tests/test_regression_aconex.py
 tests/test_regression_cl.py
 tests/test_regression_complex.py
 tests/test_regression_conex.py
 tests/test_regression_convo.py
 tests/test_regression_distmult.py
```

### Comparing `dicee-0.0.3/documents/DBpedia_experiments/ReadMe.md` & `dicee-0.0.4/documents/DBpedia_experiments/ReadMe.md`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/documents/KGEonTabular/README.md` & `dicee-0.0.4/documents/KGEonTabular/README.md`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/documents/KGEonTabular/regression.py` & `dicee-0.0.4/documents/KGEonTabular/regression.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/documents/SoftwareBenchmarks/read_csv_bencmark.py` & `dicee-0.0.4/documents/SoftwareBenchmarks/read_csv_bencmark.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/documents/using_dice_embedding_framework/Training.md` & `dicee-0.0.4/documents/using_dice_embedding_framework/Training.md`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/environment.yml` & `dicee-0.0.4/environment.yml`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/example_class_combine_kge.py` & `dicee-0.0.4/example_class_combine_kge.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/gpt.py` & `dicee-0.0.4/gpt.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/large_file_preprocessing.txt` & `dicee-0.0.4/large_file_preprocessing.txt`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/main.py` & `dicee-0.0.4/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 from dicee.executer import Execute
 import pytorch_lightning as pl
+from dicee.config import ParseDict
 import argparse
 
 def get_default_arguments(description=None):
     """ Extends pytorch_lightning Trainer's arguments with ours """
     parser = pl.Trainer.add_argparse_args(argparse.ArgumentParser(add_help=False))
     # Default Trainer param https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#methods
     parser.add_argument("--path_dataset_folder", type=str, default='KGs/UMLS',
                         help="The path of a folder containing input data")
     parser.add_argument("--save_embeddings_as_csv", type=bool, default=False,
                         help='A flag for saving embeddings in csv file.')
     parser.add_argument("--storage_path", type=str, default='Experiments',
                         help="Embeddings, model, and any other related data will be stored therein.")
     parser.add_argument("--model", type=str,
-                        default="AConEx",
-                        help="Available models: CMult, ConEx, ConvQ, ConvO, DistMult, QMult, OMult, "
-                             "Shallom, AConEx, ConEx, ComplEx, DistMult, TransE, Keci")
+                        default="Pykeen_BoxE",
+                        help="Available models: ConEx, AConEx, ConvQ, AConQ, ConvO, AConvO,QMult, OMult, Shallom, DistMult, TransE, ComplEx, Keci"
+                             "Pykeen_QuatE, Pykeen_MuRE, Pykeen_BoxE etc..")
     parser.add_argument('--optim', type=str, default='Adam',
                         help='[Adam, SGD]')
-    parser.add_argument('--embedding_dim', type=int, default=32,
+    parser.add_argument('--embedding_dim', type=int, default=16,
                         help='Number of dimensions for an embedding vector. ')
-    parser.add_argument("--num_epochs", type=int, default=100, help='Number of epochs for training. ')
+    parser.add_argument("--num_epochs", type=int, default=10, help='Number of epochs for training. ')
     parser.add_argument('--batch_size', type=int, default=1024, help='Mini batch size')
     parser.add_argument("--lr", type=float, default=0.1)
     parser.add_argument('--callbacks', '--list', nargs='+', default=[],
                         help='List of tuples representing a callback and values, e.g. [FPPE or PPE or PPE10 ,PPE20 or PPE, FPPE]')
     parser.add_argument("--backend", type=str, default='pandas',
-                        help='Select [polars(seperator: \t), modin(seperator: \s+), pandas(seperator: \s+)]')
+                        help='Select [polars(seperator: \t), pandas(seperator: \s+)]')
     parser.add_argument("--trainer", type=str, default='torchCPUTrainer',
                         help='PL (pytorch lightning trainer), torchDDP (custom ddp), torchCPUTrainer (custom cpu only)')
-    parser.add_argument('--scoring_technique', default='KvsAll', help="KvsSample, 1vsAll, KvsAll, NegSample")
-    parser.add_argument('--neg_ratio', type=int, default=0,
+    parser.add_argument('--scoring_technique', default='NegSample', help="KvsSample, 1vsAll, KvsAll, NegSample")
+    parser.add_argument('--neg_ratio', type=int, default=3,
                         help='The number of negative triples generated per positive triple.')
     parser.add_argument('--weight_decay', type=float, default=0.0, help='L2 penalty e.g.(0.00001)')
     parser.add_argument('--input_dropout_rate', type=float, default=0.0)
     parser.add_argument('--hidden_dropout_rate', type=float, default=0.0)
-    parser.add_argument("--feature_map_dropout_rate", type=int, default=0.0)
+    parser.add_argument("--feature_map_dropout_rate", type=float, default=0.0)
     parser.add_argument("--normalization", type=str, default="None", help="[LayerNorm, BatchNorm1d, None]")
     parser.add_argument("--init_param", type=str, default=None, help="[xavier_normal, None]")
     parser.add_argument("--gradient_accumulation_steps", type=int, default=0,
                         help="e.g. gradient_accumulation_steps=2 implies that gradients are accumulated at every second mini-batch")
     parser.add_argument('--num_folds_for_cv', type=int, default=0,
                         help='Number of folds in k-fold cross validation.'
                              'If >2 ,no evaluation scenario is applied implies no evaluation.')
     parser.add_argument("--eval_model", type=str, default="train_val_test",
-                        help='train, val, test, constraint, combine them anyway you want, e.g. '
+                        help='test the link prediction results on the splits, e.g. '
                              'train_val,train_val_test, val_test, val_test_constraint ')
     parser.add_argument("--save_model_at_every_epoch", type=int, default=None,
                         help='At every X number of epochs model will be saved. If None, we save 4 times.')
     parser.add_argument("--label_smoothing_rate", type=float, default=0.0, help='None for not using it.')
-    parser.add_argument("--kernel_size", type=int, default=3, help="Square kernel size for ConEx")
+    parser.add_argument("--kernel_size", type=int, default=3, help="Square kernel size for convolution based models.")
     parser.add_argument("--num_of_output_channels", type=int, default=2,
                         help="# of output channels in convolution")
-    parser.add_argument("--num_core", type=int, default=0,
+    parser.add_argument("--num_core", type=int, default=4,
                         help='Number of cores to be used. 0 implies using single CPU')
     parser.add_argument("--seed_for_computation", type=int, default=0,
                         help='Seed for all, see pl seed_everything().')
     parser.add_argument("--sample_triples_ratio", type=float, default=None, help='Sample input data.')
     parser.add_argument("--read_only_few", type=int, default=None,
                         help='READ only first N triples. If 0, read all.')
     parser.add_argument('--p', type=int, default=0,
                         help='P for Clifford Algebra')
     parser.add_argument('--q', type=int, default=0,
                         help='Q for Clifford Algebra')
     parser.add_argument('--auto_batch_finder', type=bool, default=False,
                         help='Find a batch size w.r.t. computational budgets')
+    parser.add_argument("--pykeen_model_kwargs", nargs='*', action=ParseDict,
+                        default={},
+                        help='Additional parameters to be passed into a knowledge graph embedding model imported from Pykeen')
     if description is None:
         return parser.parse_args()
     return parser.parse_args(description)
 
 
 if __name__ == '__main__':
     Execute(get_default_arguments()).start()
```

### Comparing `dicee-0.0.3/meta_heuristic.py` & `dicee-0.0.4/meta_heuristic.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/out_of_sample.py` & `dicee-0.0.4/out_of_sample.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/plot.py` & `dicee-0.0.4/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+from dicee import KGE
+
+KGE('Experiments/2023-05-12 10:27:13.950047')
+
+exit(1)
 import os
 import json
 import pandas as pd
 import pickle
 import matplotlib.pyplot as plt
 
 paths = ['UMLS/', 'KINSHIP/']
```

### Comparing `dicee-0.0.3/self_attention.py` & `dicee-0.0.4/self_attention.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/setup.py` & `dicee-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 setup(
     name='dicee',
     description='Dice embedding is an hardware-agnostic framework for large-scale knowledge graph embedding applications',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
-    install_requires=['pandas>=1.5.1',
-                      "polars>=0.16.14",
-                      "pyarrow>=11.0.0",
-                      'torch>=2.0.0',
-                      "pytorch-lightning==1.6.4",
-                      "scikit-learn>=1.2.2",
-                      "pytest>=7.2.2",
-                      "psutil>=5.9.4",
-                      "gradio>=3.23.0"],
+    install_requires=[
+        "torch>=2.0.0",
+        "pandas>=1.5.1",
+        "polars>=0.16.14",
+        "scikit-learn>=1.2.2",
+        "pyarrow>=11.0.0",
+        "pytorch-lightning==1.6.4",
+        "pykeen==1.10.1",
+        "zstandard>=0.21.0",
+        "pytest>=7.2.2",
+        "psutil>=5.9.4",
+        "gradio>=3.23.0"],
     author='Caglar Demir',
     author_email='caglardemir8@gmail.com',
     url='https://github.com/dice-group/dice-embeddings',
     classifiers=[
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License"],
     python_requires='>=3.10',
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `dicee-0.0.3/tests/test_auto_batch_finder.py` & `dicee-0.0.4/tests/test_auto_batch_finder.py`

 * *Files identical despite different names*

### Comparing `dicee-0.0.3/tests/test_conjuncive_query_answering.py` & `dicee-0.0.4/tests/test_conjuncive_query_answering.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 import os
 
 
 class TestKGEInteractive:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_missing_triples_and_conjunctive_query_answering(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
```

### Comparing `dicee-0.0.3/tests/test_continual_training.py` & `dicee-0.0.4/tests/test_continual_training.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 import os
 
 
 class TestRegressionCL:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
@@ -31,15 +31,15 @@
         assert os.path.isdir(result['path_experiment_folder'])
         pre_trained_kge = KGE(path=result['path_experiment_folder'])
         kg = KG(data_dir=args.path_dataset_folder)
         pre_trained_kge.train(kg, epoch=1, batch_size=args.batch_size)
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling_Family(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.path_dataset_folder = 'KGs/Family'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.num_epochs = 1
         args.batch_size = 1024
         args.lr = 0.1
```

### Comparing `dicee-0.0.3/tests/test_custom_trainer.py` & `dicee-0.0.4/tests/test_custom_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dicee.config import Args
 import pytest
 
 
 class TestDefaultParams:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_shallom(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'Shallom'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -22,15 +22,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -42,15 +42,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -61,15 +61,15 @@
         args.read_only_few = None
         args.sample_triples_ratio = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convq(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'ConvQ'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -81,15 +81,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_omult(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.num_epochs = 1
         args.scoring_technique = 'NegSample'
         args.neg_ratio = 1
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
@@ -102,15 +102,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convo(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.num_epochs = 1
         args.scoring_technique = 'NegSample'
         args.neg_ratio = 1
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
@@ -122,15 +122,15 @@
         args.sample_triples_ratio = None
         args.read_only_few = None
         args.sample_triples_ratio = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     def test_distmult(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.num_epochs = 1
         args.scoring_technique = 'NegSample'
         args.neg_ratio = 1
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
```

### Comparing `dicee-0.0.3/tests/test_deployment.py` & `dicee-0.0.4/tests/test_gradient_accumulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 from dicee.executer import Execute
 import sys
 import pytest
-from dicee import KGE
-from dicee.static_funcs import random_prediction
 from dicee.config import Args
 
 class TestDefaultParams:
     @pytest.mark.filterwarnings('ignore::UserWarning')
-    def test_qmult(self):
-        args = Args()#get_default_arguments([])
-        args.model = 'QMult'
-        args.optim = 'Adam'
+    def test_shallom(self):
+        args = Args()
+        args.model = 'Shallom'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
         args.hidden_dropout_rate = 0.0
         args.feature_map_dropout_rate = 0.0
         args.sample_triples_ratio = None
         args.read_only_few = None
-        args.backend = 'pandas'
-        args.sample_triples_ratio = None
+        args.num_folds_for_cv = None
+        args.gradient_accumulation_steps = 5
         args.trainer = 'torchCPUTrainer'
-        executor = Execute(args)
-        executor.start()
-
-        pre_trained_kge = KGE(path=executor.args.full_storage_path)
-        random_prediction(pre_trained_kge)
+        Execute(args).start()
```

### Comparing `dicee-0.0.3/tests/test_different_backends.py` & `dicee-0.0.4/tests/test_different_backends.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         args = get_default_arguments([])
         args.path_dataset_folder = 'KGs/UMLS'
         args.backend = 'pandas'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_pandas_as_backend(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.path_dataset_folder = 'KGs/UMLS'
         args.backend = 'polars'
         Execute(args).start()
```

### Comparing `dicee-0.0.3/tests/test_ensemble_construction.py` & `dicee-0.0.4/tests/test_ensemble_construction.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 import os
 from dicee.config import Args
 
 class TestEnsembleConstruction:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
```

### Comparing `dicee-0.0.3/tests/test_execute_start.py` & `dicee-0.0.4/tests/test_execute_start.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 from dicee.config import Args
 
 
 class TestDefaultParams:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_shallom(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'Shallom'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -23,15 +23,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -43,15 +43,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -63,15 +63,15 @@
         args.read_only_few = None
         args.sample_triples_ratio = None
         args.trainer = None
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convq(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvQ'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -83,15 +83,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_omult(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -103,15 +103,15 @@
         args.read_only_few = None
         args.num_folds_for_cv = None
         args.trainer = None
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convo(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -122,15 +122,15 @@
         args.sample_triples_ratio = None
         args.read_only_few = None
         args.sample_triples_ratio = None
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     def test_distmult(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
```

### Comparing `dicee-0.0.3/tests/test_k_fold_cv_1_vs_all.py` & `dicee-0.0.4/tests/test_k_fold_cv_1_vs_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 from dicee.config import Args
 
 class TestCV_1vsAll:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_shallom_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'Shallom'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -24,15 +24,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.eval_model = 'test'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -46,15 +46,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.eval_model = 'test'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -68,15 +68,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.eval_model = 'test'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convq_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvQ'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -90,15 +90,15 @@
         args.eval_model = 'test'
         args.num_folds_for_cv = 3
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_omult_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -112,15 +112,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convo_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -133,15 +133,15 @@
         args.eval_model = 'test'
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.num_folds_for_cv = 3
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     def test_distmult_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -154,15 +154,15 @@
         args.eval_model = 'test'
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.num_folds_for_cv = 3
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     def test_complex_1vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ComplEx'
         args.num_epochs = 1
         args.scoring_technique = '1vsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
```

### Comparing `dicee-0.0.3/tests/test_k_fold_cv_k_vs_all.py` & `dicee-0.0.4/tests/test_k_fold_cv_k_vs_all.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestCV_KvsAll:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_shallom_kvs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'Shallom'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -23,15 +23,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex_kvs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -45,15 +45,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult_kvs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -67,15 +67,15 @@
         args.backend = 'pandas'  # Error with polars because sep="\s" should be a single byte character, but is 2 bytes long.
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convq_kvs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvQ'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -89,15 +89,15 @@
         args.backend = 'pandas'  # Error with polars becasue sep="\s" should be a single byte character, but is 2 bytes long.
         args.num_folds_for_cv = 3
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_omult_kvs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -111,15 +111,15 @@
         args.eval_model = 'train'
         args.num_folds_for_cv = 3
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convo_kvs_all(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -130,15 +130,15 @@
         args.eval_model = 'train'
         args.backend = 'pandas'  # Error with polars becasue sep="\s" should be a single byte character, but is 2 bytes long.
         args.num_folds_for_cv = 3
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     def test_distmult_kvs_all(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
@@ -148,15 +148,15 @@
         args.eval_model = 'train'
         args.num_folds_for_cv = 3
         args.backend = 'pandas'  # Error with polars becasue sep="\s" should be a single byte character, but is 2 bytes long.
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     def test_complex_kvs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ComplEx'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/Family'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
```

### Comparing `dicee-0.0.3/tests/test_k_fold_cv_neg_sample.py` & `dicee-0.0.4/tests/test_k_fold_cv_neg_sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 from dicee.config import Args
 
 class TestCV_NegSample:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex_NegSample(self):
-        args = Args()#get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.num_epochs = 1
         args.scoring_technique = 'NegSample'
         args.neg_ratio = 1
         args.path_dataset_folder = 'KGs/Family'
         args.batch_size = 1024
         args.lr = 0.01
@@ -19,15 +19,15 @@
         args.eval_model = 'train'
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult_NegSample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.num_epochs = 1
         args.scoring_technique = 'NegSample'
         args.neg_ratio = 1
         args.path_dataset_folder = 'KGs/Family'
         args.batch_size = 1024
         args.lr = 0.01
@@ -36,15 +36,15 @@
         args.eval_model = 'train'
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convq_NegSample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvQ'
         args.scoring_technique = 'NegSample'
         args.path_dataset_folder = 'KGs/Family'
         args.neg_ratio = 1
         args.num_epochs = 1
         args.batch_size = 1024
         args.lr = 0.01
@@ -53,15 +53,15 @@
         args.eval_model = 'train'
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_omult_NegSample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.num_epochs = 1
         args.scoring_technique = 'NegSample'
         args.path_dataset_folder = 'KGs/Family'
         args.neg_ratio = 1
         args.batch_size = 1024
         args.lr = 0.01
@@ -70,30 +70,30 @@
         args.eval_model = 'train'
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_convo_NegSample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.scoring_technique = 'NegSample'
         args.path_dataset_folder = 'KGs/Family'
         args.neg_ratio = 1
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.backend = 'pandas'  #  Error with polars becasue sep="\s" should be a single byte character, but is 2 bytes long.
         args.eval_model = 'train'
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     def test_distmult_NegSample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.scoring_technique = 'NegSample'
         args.path_dataset_folder = 'KGs/Family'
         args.neg_ratio = 1
         args.num_epochs = 1
         args.batch_size = 1024
         args.lr = 0.01
@@ -101,15 +101,15 @@
         args.backend = 'pandas'  #  Error with polars becasue sep="\s" should be a single byte character, but is 2 bytes long.
         args.eval_model = 'train'
         args.trainer = 'torchCPUTrainer'
         args.num_folds_for_cv = 3
         Execute(args).start()
 
     def test_complex_NegSample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ComplEx'
         args.scoring_technique = 'NegSample'
         args.path_dataset_folder = 'KGs/Family'
         args.neg_ratio = 1
         args.num_epochs = 1
         args.batch_size = 1024
         args.lr = 0.01
```

### Comparing `dicee-0.0.3/tests/test_kvssample.py` & `dicee-0.0.4/tests/test_kvssample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionQmult:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_sample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.path_dataset_folder = 'KGs/UMLS'
         args.optim = 'Adam'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -28,15 +28,15 @@
 
         assert result['Train']['H@10'] >= result['Train']['H@3'] >= result['Train']['H@1']
         assert result['Val']['H@10'] >= result['Val']['H@3'] >= result['Val']['H@1']
         assert result['Test']['H@10'] >= result['Test']['H@3'] >= result['Test']['H@1']
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_sample_regression(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.path_dataset_folder = 'KGs/UMLS'
         args.optim = 'Adam'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
         args.embedding_dim = 32
```

### Comparing `dicee-0.0.3/tests/test_large_kg.py` & `dicee-0.0.4/tests/test_large_kg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionDistMult:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.path_dataset_folder = 'KGs/WN18RR'
         args.optim = 'Adam'
         args.num_epochs = 0
         args.batch_size = 32
         args.lr = 0.1
         args.embedding_dim = 32
@@ -27,15 +27,15 @@
         args.scoring_technique = 'KvsAll'
         result = Execute(args).start()
         assert 0.03 >= result['Val']['MRR'] >= 0.0002
         assert 0.03 >= result['Test']['MRR'] >= 0.0002
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_neg_sample(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.path_dataset_folder = 'KGs/WN18RR'
         args.optim = 'Adam'
         args.num_epochs = 0
         args.batch_size = 32
         args.lr = 0.1
         args.embedding_dim = 32
```

### Comparing `dicee-0.0.3/tests/test_online_learning.py` & `dicee-0.0.4/tests/test_online_learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 import os
 from dicee.config import Args
 
 class TestRegressionOnlineLearning:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_umls(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.scoring_technique = 'KvsSample'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 0
         args.batch_size = 1024
         args.lr = 0.1
```

### Comparing `dicee-0.0.3/tests/test_pickle.py` & `dicee-0.0.4/tests/test_pickle.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 import pickle
 import pytest
 from dicee.config import Args
 
 class TestPickle:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_dismult_pickle(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.path_dataset_folder = 'KGs/UMLS'
         args.model = 'DistMult'
         executor = Execute(args)
         args.scoring_technique = 'NegSample'
         args.trainer = 'torchCPUTrainer'
         executor.start()
         pickle.dump(executor.trained_model, open("trained_model.p", "wb"))
         pickled_trained_model = pickle.load(open("trained_model.p", "rb"))
         os.remove('trained_model.p')
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_transe_pickle(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.path_dataset_folder = 'KGs/UMLS'
         args.model = 'TransE'
         args.scoring_technique = 'NegSample'
         executor = Execute(args)
         args.trainer = 'torchCPUTrainer'
         executor.start()
         pickle.dump(executor.trained_model, open("trained_model.p", "wb"))
         pickled_trained_model = pickle.load(open("trained_model.p", "rb"))
         os.remove('trained_model.p')
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult_pickle(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.path_dataset_folder = 'KGs/UMLS'
         args.model = 'QMult'
         args.embedding_dim = 16
         args.scoring_technique = 'NegSample'
         executor = Execute(args)
         args.trainer = 'torchCPUTrainer'
         executor.start()
@@ -56,15 +56,15 @@
         executor.start()
         pickle.dump(executor.trained_model, open("trained_model.p", "wb"))
         pickled_trained_model = pickle.load(open("trained_model.p", "rb"))
         os.remove('trained_model.p')
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex_pickle(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.path_dataset_folder = 'KGs/UMLS'
         args.model = 'ConEx'
         args.scoring_technique = 'NegSample'
         executor = Execute(args)
         args.trainer = 'torchCPUTrainer'
         executor.start()
         pickle.dump(executor.trained_model, open("trained_model.p", "wb"))
```

### Comparing `dicee-0.0.3/tests/test_read_few_only.py` & `dicee-0.0.4/tests/test_read_few_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 from dicee.config import Args
 
 class TestReadFewOnly:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_qmult_kvsall(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
```

### Comparing `dicee-0.0.3/tests/test_regression_aconex.py` & `dicee-0.0.4/tests/test_regression_aconex.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 from dicee.config import Args
 
 class TestRegressionAConEx:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
```

### Comparing `dicee-0.0.3/tests/test_regression_cl.py` & `dicee-0.0.4/tests/test_regression_cl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute, ContinuousExecute
 import pytest
 from dicee.config import Args
 
 class TestRegressionAConEx:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.scoring_technique = 'KvsSample'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 5
         args.batch_size = 4096
         args.lr = 0.1
```

### Comparing `dicee-0.0.3/tests/test_regression_complex.py` & `dicee-0.0.4/tests/test_regression_complex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionComplEx:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ComplEx'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
@@ -27,15 +27,15 @@
         result = Execute(args).start()
         assert 0.84 >= result['Train']['H@1'] >= 0.75
         assert 0.84 >= result['Val']['H@1'] >= 0.60
         assert 0.84 >= result['Test']['H@1'] >= 0.60
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_1_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ComplEx'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
@@ -52,15 +52,15 @@
         result = Execute(args).start()
         assert 1.0 >= result['Train']['H@1'] >= 0.30
         assert 0.87 >= result['Val']['H@1'] >= 0.15
         assert 0.87 >= result['Test']['H@1'] >= 0.15
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ComplEx'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
```

### Comparing `dicee-0.0.3/tests/test_regression_conex.py` & `dicee-0.0.4/tests/test_regression_conex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionConEx:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.scoring_technique = 'KvsAll'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 20
         args.batch_size = 1024
         args.lr = 0.01
@@ -27,15 +27,15 @@
         result = Execute(args).start()
         assert 0.46 >= result['Train']['H@1'] >= 0.32
         assert 0.46 >= result['Val']['H@1'] >= 0.32
         assert 0.46 >= result['Test']['H@1'] >= 0.30
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_1_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
@@ -52,15 +52,15 @@
         result = Execute(args).start()
         assert 0.75 >= result['Train']['H@1'] > 0.02
         assert 0.75 >= result['Val']['H@1'] >= 0.02
         assert 0.75 >= result['Test']['H@1'] >= 0.02
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConEx'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
@@ -75,7 +75,9 @@
         args.normalization = 'LayerNorm'
         args.trainer = 'torchCPUTrainer'
         args.init_param = 'xavier_normal'
         result = Execute(args).start()
         assert 0.77 >= result['Train']['H@1'] >= .20
         assert 0.70 >= result['Val']['H@1'] >= .20
         assert 0.70 >= result['Test']['H@1'] >= .20
+
+    # TODO: Write Test and compare ConEx with AConEx
```

### Comparing `dicee-0.0.3/tests/test_regression_convo.py` & `dicee-0.0.4/tests/test_regression_convo.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 from dicee.config import Args
 
 class TestRegressionConvO:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
         args.embedding_dim = 32
@@ -24,15 +24,15 @@
         args.normalization = 'LayerNorm'
         args.init_param = 'xavier_normal'
         args.trainer = 'torchCPUTrainer'
         result = Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_1_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.1
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
@@ -47,15 +47,15 @@
         args.trainer = 'torchCPUTrainer'
         args.scoring_technique = '1vsAll'
         result = Execute(args).start()
 
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'ConvO'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.eval_model = 'train_val_test'
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
```

### Comparing `dicee-0.0.3/tests/test_regression_distmult.py` & `dicee-0.0.4/tests/test_regression_distmult.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionDistMult:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -24,15 +24,15 @@
         args.init_param = 'xavier_normal'
         args.trainer = 'torchCPUTrainer'
         result = Execute(args).start()
         assert 0.58 >= result['Val']['H@1'] >= 0.01
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_1_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
@@ -46,15 +46,15 @@
         args.normalization = 'LayerNorm'
         args.init_param = 'xavier_normal'
         args.trainer = 'torchCPUTrainer'
         result = Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'DistMult'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.input_dropout_rate = 0.0
```

### Comparing `dicee-0.0.3/tests/test_regression_omult.py` & `dicee-0.0.4/tests/test_regression_omult.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionOmult:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -26,15 +26,15 @@
         args.trainer = 'torchCPUTrainer'
         result = Execute(args).start()
         assert 0.90 >= result['Train']['H@1'] >= 0.65
         assert 0.76 >= result['Val']['H@1'] >= 0.70
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_1_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -53,15 +53,15 @@
         result = Execute(args).start()
         assert 0.75 >= result['Test']['H@1'] >= 0.71
         assert 0.78 >= result['Val']['H@1'] >= 0.74
         assert 0.92 >= result['Train']['H@1'] >= 0.82
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'OMult'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
```

### Comparing `dicee-0.0.3/tests/test_regression_polyak.py` & `dicee-0.0.4/tests/test_regression_polyak.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import pytest
 from dicee.config import Args
 
 class TestPolyak:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_polyak_qmult_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.path_dataset_folder = 'KGs/UMLS'
         args.optim = 'Adam'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -32,15 +32,15 @@
         assert 0.640 >= result['Test']['H@1'] >= 0.620
         assert result['Train']['H@10'] >= result['Train']['H@3'] >= result['Train']['H@1']
         assert result['Val']['H@10'] >= result['Val']['H@3'] >= result['Val']['H@1']
         assert result['Test']['H@10'] >= result['Test']['H@3'] >= result['Test']['H@1']
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_polyak_qmult_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.path_dataset_folder = 'KGs/UMLS'
         args.optim = 'Adam'
         args.num_epochs = 59
         args.batch_size = 1024
         args.lr = 0.1
         args.callbacks = ['FPPE']
```

### Comparing `dicee-0.0.3/tests/test_regression_pyke.py` & `dicee-0.0.4/tests/test_regression_pyke.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionPyke:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'Pyke'
         args.path_dataset_folder = 'KGs/UMLS'
         args.optim = 'Adam'
         args.num_epochs = 5
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
```

### Comparing `dicee-0.0.3/tests/test_regression_qmult.py` & `dicee-0.0.4/tests/test_regression_qmult.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dicee.executer import Execute
 import pytest
 from dicee.config import Args
 
 class TestRegressionQmult:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_k_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.path_dataset_folder = 'KGs/UMLS'
         args.optim = 'Adam'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -30,15 +30,15 @@
 
         assert result['Train']['H@10'] >= result['Train']['H@3'] >= result['Train']['H@1']
         assert result['Val']['H@10'] >= result['Val']['H@3'] >= result['Val']['H@1']
         assert result['Test']['H@10'] >= result['Test']['H@3'] >= result['Test']['H@1']
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_1_vs_all(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
@@ -59,15 +59,15 @@
 
         assert result['Train']['H@10'] >= result['Train']['H@3'] >= result['Train']['H@1']
         assert result['Val']['H@10'] >= result['Val']['H@3'] >= result['Val']['H@1']
         assert result['Test']['H@10'] >= result['Test']['H@3'] >= result['Test']['H@1']
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_negative_sampling(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'QMult'
         args.optim = 'Adam'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 50
         args.batch_size = 1024
         args.lr = 0.1
         args.embedding_dim = 32
```

### Comparing `dicee-0.0.3/tests/test_trainers.py` & `dicee-0.0.4/tests/test_trainers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from dicee.executer import Execute
 from dicee.config import Args
 import pytest
 
 class TestCallback:
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_conex_torch_cpu_trainer(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
         args.embedding_dim = 32
         args.trainer = 'torchCPUTrainer'
         Execute(args).start()
 
     @pytest.mark.filterwarnings('ignore::UserWarning')
     def test_aconex_pl_trainer(self):
-        args = Args()  # get_default_arguments([])
+        args = Args()
         args.model = 'AConEx'
         args.num_epochs = 1
         args.scoring_technique = 'KvsAll'
         args.path_dataset_folder = 'KGs/UMLS'
         args.num_epochs = 10
         args.batch_size = 1024
         args.lr = 0.01
```

