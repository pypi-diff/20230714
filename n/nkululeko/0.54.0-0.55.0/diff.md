# Comparing `tmp/nkululeko-0.54.0.tar.gz` & `tmp/nkululeko-0.55.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.54.0.tar", last modified: Thu Jul 13 17:31:00 2023, max compression
+gzip compressed data, was "nkululeko-0.55.0.tar", last modified: Fri Jul 14 19:48:24 2023, max compression
```

## Comparing `nkululeko-0.54.0.tar` & `nkululeko-0.55.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-13 17:31:00.682561 nkululeko-0.54.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7285 2023-07-13 17:27:18.000000 nkululeko-0.54.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.54.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19069 2023-07-13 17:31:00.682561 nkululeko-0.54.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11232 2023-07-12 17:10:33.000000 nkululeko-0.54.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-13 17:31:00.682561 nkululeko-0.54.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.54.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.54.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.54.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.54.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.54.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-13 17:01:55.000000 nkululeko-0.54.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.54.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.54.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.54.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.54.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.54.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21808 2023-07-11 17:10:58.000000 nkululeko-0.54.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.54.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2751 2023-07-13 17:19:32.000000 nkululeko-0.54.0/nkululeko/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2832 2023-07-13 17:19:11.000000 nkululeko-0.54.0/nkululeko/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.54.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2750 2023-07-13 17:19:46.000000 nkululeko-0.54.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2741 2023-07-13 17:20:04.000000 nkululeko-0.54.0/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.54.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.54.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.54.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.54.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.54.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.54.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.54.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.54.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3935 2023-07-13 17:17:52.000000 nkululeko-0.54.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.54.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.54.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3510 2023-07-11 17:13:59.000000 nkululeko-0.54.0/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6717 2023-07-11 16:16:04.000000 nkululeko-0.54.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.54.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.54.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.54.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.54.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.54.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.54.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.54.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.54.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.54.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.54.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.54.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.54.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.54.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.54.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.54.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.54.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.54.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.54.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.54.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.54.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.54.0/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.54.0/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.54.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.54.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.54.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.54.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.54.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.54.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.54.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10463 2023-07-06 09:40:02.000000 nkululeko-0.54.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-13 17:31:00.682561 nkululeko-0.54.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19069 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1737 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-13 17:31:00.000000 nkululeko-0.54.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.54.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-13 17:31:00.682561 nkululeko-0.54.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.54.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-14 19:48:24.734564 nkululeko-0.55.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7344 2023-07-14 18:30:19.000000 nkululeko-0.55.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.55.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19325 2023-07-14 19:48:24.734564 nkululeko-0.55.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11429 2023-07-14 19:31:57.000000 nkululeko-0.55.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-14 19:48:24.730564 nkululeko-0.55.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.55.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.55.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.55.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.55.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.55.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-14 18:29:54.000000 nkululeko-0.55.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.55.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.55.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.55.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.55.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.55.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21914 2023-07-14 18:19:14.000000 nkululeko-0.55.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.55.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2751 2023-07-13 17:19:32.000000 nkululeko-0.55.0/nkululeko/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2832 2023-07-13 17:19:11.000000 nkululeko-0.55.0/nkululeko/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.55.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2750 2023-07-13 17:19:46.000000 nkululeko-0.55.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2741 2023-07-13 17:20:04.000000 nkululeko-0.55.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.55.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.55.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.55.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.55.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.55.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.55.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.55.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.55.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3935 2023-07-13 17:17:52.000000 nkululeko-0.55.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.55.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.55.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3510 2023-07-11 17:13:59.000000 nkululeko-0.55.0/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6717 2023-07-11 16:16:04.000000 nkululeko-0.55.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.55.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.55.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.55.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.55.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.55.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.55.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.55.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.55.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.55.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.55.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.55.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.55.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.55.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.55.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.55.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.55.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.55.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.55.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.55.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.55.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.55.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.55.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.55.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.55.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.55.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.55.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3928 2023-07-14 19:27:37.000000 nkululeko-0.55.0/nkululeko/segment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.55.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.55.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.55.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9480 2023-07-14 18:17:36.000000 nkululeko-0.55.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-14 19:48:24.734564 nkululeko-0.55.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19325 2023-07-14 19:48:24.000000 nkululeko-0.55.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1758 2023-07-14 19:48:24.000000 nkululeko-0.55.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-14 19:48:24.000000 nkululeko-0.55.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-14 19:48:24.000000 nkululeko-0.55.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-14 19:48:24.000000 nkululeko-0.55.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.55.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-14 19:48:24.734564 nkululeko-0.55.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.55.0/setup.py
```

### Comparing `nkululeko-0.54.0/CHANGELOG.md` & `nkululeko-0.55.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.55.0
+--------------
+* added segmentation module
+
 Version 0.54.0
 --------------
 * added audeering public age and gender model embeddings and age and gender predictions
 
 Version 0.53.0
 --------------
 * added file checks: size in bytes and voice activity detection with silero
```

### Comparing `nkululeko-0.54.0/LICENSE` & `nkululeko-0.55.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/PKG-INFO` & `nkululeko-0.55.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.54.0
+Version: 0.55.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,16 +137,18 @@
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
- * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
- * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
+* [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
+* [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
+* [Check your dataset](http://blog.syntheticspeech.de/2023/07/11/nkululeko-check-your-dataset/) 
+* [Segmenting a database](http://blog.syntheticspeech.de/2023/07/14/nkululeko-segmenting-a-database/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework (and [here's the real one done with pyreverse](meta/images/classes.png)).
 ![sketch](meta/images/class_diagram.png)
 
 
@@ -211,14 +213,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.55.0
+--------------
+* added segmentation module
+
 Version 0.54.0
 --------------
 * added audeering public age and gender model embeddings and age and gender predictions
 
 Version 0.53.0
 --------------
 * added file checks: size in bytes and voice activity detection with silero
```

### Comparing `nkululeko-0.54.0/README.md` & `nkululeko-0.55.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,18 @@
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
- * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
- * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
+* [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
+* [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
+* [Check your dataset](http://blog.syntheticspeech.de/2023/07/11/nkululeko-check-your-dataset/) 
+* [Segmenting a database](http://blog.syntheticspeech.de/2023/07/14/nkululeko-segmenting-a-database/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework (and [here's the real one done with pyreverse](meta/images/classes.png)).
 ![sketch](meta/images/class_diagram.png)
```

### Comparing `nkululeko-0.54.0/nkululeko/augment.py` & `nkululeko-0.55.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/augmenter.py` & `nkululeko-0.55.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/cacheddataset.py` & `nkululeko-0.55.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/dataset.py` & `nkululeko-0.55.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/dataset_csv.py` & `nkululeko-0.55.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.55.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/demo.py` & `nkululeko-0.55.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/demo_predictor.py` & `nkululeko-0.55.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/experiment.py` & `nkululeko-0.55.0/nkululeko/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         ----------
         config_obj : a config parser object that sets the experiment parameters and being set as a global object.
         """
 
         self.set_globals(config_obj)
         self.name = glob_conf.config['EXP']['name']
         self.root = glob_conf.config['EXP']['root']
-        audeer.mkdir(self.root+self.name) # create the experiment directory
+        self.data_dir = self.root+self.name
+        audeer.mkdir(self.data_dir) # create the experiment directory
         self.util = Util('experiment')
         glob_conf.set_util(self.util)
         self.loso = self.util.config_val('MODEL', 'loso', False)
         self.logo = self.util.config_val('MODEL', 'logo', False)
         self.xfoldx = self.util.config_val('MODEL', 'k_fold_cross', False)
         self.start = time.process_time()
 
@@ -77,14 +78,15 @@
                 self.got_gender = True
             if data.got_age:
                 self.got_age = True
             if data.got_speaker:
                 self.got_speaker = True
             self.datasets.update({d: data})
         self.target = self.util.config_val('DATA', 'target', 'emotion')
+        self.util.debug(f'loaded {self.datasets.keys()} databases')
 
     def _import_csv(self, storage):
         # df = pd.read_csv(storage, header=0, index_col=[0,1,2])
         # df.index.set_levels(pd.to_timedelta(df.index.levels[1]), level=1)
         # df.index.set_levels(pd.to_timedelta(df.index.levels[2]), level=2)
         df = audformat.utils.read_csv(storage)
         df.is_labeled = True if self.target in df else False
```

### Comparing `nkululeko-0.54.0/nkululeko/explore.py` & `nkululeko-0.55.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_agender.py` & `nkululeko-0.55.0/nkululeko/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_agender_agender.py` & `nkululeko-0.55.0/nkululeko/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_analyser.py` & `nkululeko-0.55.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_audmodel.py` & `nkululeko-0.55.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.55.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_clap.py` & `nkululeko-0.55.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_import.py` & `nkululeko-0.55.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_mld.py` & `nkululeko-0.55.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_opensmile.py` & `nkululeko-0.55.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_oxbow.py` & `nkululeko-0.55.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_praat.py` & `nkululeko-0.55.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_trill.py` & `nkululeko-0.55.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.55.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feature_extractor.py` & `nkululeko-0.55.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/featureset.py` & `nkululeko-0.55.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/feinberg_praat.py` & `nkululeko-0.55.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/file_checker.py` & `nkululeko-0.55.0/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/filter_data.py` & `nkululeko-0.55.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/loss_ccc.py` & `nkululeko-0.55.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.55.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model.py` & `nkululeko-0.55.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_cnn.py` & `nkululeko-0.55.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_gmm.py` & `nkululeko-0.55.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_knn.py` & `nkululeko-0.55.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_knn_reg.py` & `nkululeko-0.55.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_mlp.py` & `nkululeko-0.55.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.55.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/model_svm.py` & `nkululeko-0.55.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/modelrunner.py` & `nkululeko-0.55.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/nkululeko.py` & `nkululeko-0.55.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/plots.py` & `nkululeko-0.55.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/randomsplicer.py` & `nkululeko-0.55.0/nkululeko/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/randomsplicing.py` & `nkululeko-0.55.0/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/reporter.py` & `nkululeko-0.55.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/runmanager.py` & `nkululeko-0.55.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/scaler.py` & `nkululeko-0.55.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.55.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/test.py` & `nkululeko-0.55.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/test_predictor.py` & `nkululeko-0.55.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.54.0/nkululeko/util.py` & `nkululeko-0.55.0/nkululeko/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -78,16 +78,14 @@
                     if not default in self.stopvals:
                         self.debug(f'value for {key} not found, using default: {default}')
                     return default
             if not default in self.stopvals:
                 self.debug(f'value for {key} not found, using default: {default}')
             return default
 
-
-
     def get_save_name(self):
         """Return a relative path to a name to save the experiment"""
         store = self.get_path('store')
         return f'{store}/{self.get_exp_name()}.pkl'
 
     def is_categorical(self, pd_series):
         """Check if a dataframe column is categorical"""
@@ -130,45 +128,27 @@
             mt = f'_{glob_conf.config["MODEL"]["type"]}'
         ft = '_'.join(ast.literal_eval(glob_conf.config['FEATS']['type']))
         ft += '_'
         set = self.config_val('FEATS', 'set', False)
         set_string = ''
         if set:
             set_string += set
-        # lr_string = ''
-        # if self.config_val('MODEL', 'learning_rate', False) and not only_data:
-        #     lr = self.config_val('MODEL', 'learning_rate', False)
-        #     lr_string = f'_lr-{str(lr)}'
-        # logo_string = ''
-        # if self.config_val('MODEL', 'logo', False):
-        #     logo = self.config_val('MODEL', 'logo', False)
-        #     logo_string = f'_logo-{str(logo)}'
-        # loss_string = ''
-        # if self.config_val('MODEL', 'loss', False) and not only_data:
-        #     loss = self.config_val('MODEL', 'loss', False)
-        #     loss_string = f'_loss-{loss}'
-        # drop_string = ''
-        # if self.config_val('MODEL', 'drop', False) and not only_data:
-        #     drop = self.config_val('MODEL', 'drop', False)
-        #     drop_string = f'_drop-{str(drop)}'
         layer_string = ''
         layer_s = self.config_val('MODEL', 'layers', False)
         if layer_s and not only_data:
             layers = ast.literal_eval(layer_s)
             sorted_layers = sorted(layers.items(), key=lambda x: x[1])
             for l in sorted_layers:
                 layer_string += f'{str(l[1])}-'
         return_string = f'{ds}{mt}_{ft}{set_string}'\
             f'{layer_string[:-1]}'
         options = [['MODEL', 'drop'], ['MODEL', 'loss'], ['MODEL', 'logo'], 
                    ['MODEL', 'learning_rate'],  ['MODEL', 'k_fold_cross']]
         for option in options:
             return_string += self._get_value_descript(option[0], option[1])
-        # return_string = f'{ds}{mt}_{ft}{set_string}'\
-        #     f'{layer_string[:-1]}{lr_string}{drop_string}{loss_string}{logo_string}'.replace('__','')
         return return_string.replace('__','')
 
     def get_plot_name(self):
         try:
             plot_name = glob_conf.config['PLOT']['name']
         except KeyError:
             plot_name = self.get_exp_name()
```

### Comparing `nkululeko-0.54.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.55.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.54.0
+Version: 0.55.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,16 +137,18 @@
 * [Run multiple experiments in one go](http://blog.syntheticspeech.de/2022/03/28/how-to-run-multiple-experiments-in-one-go-with-nkululeko/)
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
- * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
- * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
+* [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
+* [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
+* [Check your dataset](http://blog.syntheticspeech.de/2023/07/11/nkululeko-check-your-dataset/) 
+* [Segmenting a database](http://blog.syntheticspeech.de/2023/07/14/nkululeko-segmenting-a-database/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework (and [here's the real one done with pyreverse](meta/images/classes.png)).
 ![sketch](meta/images/class_diagram.png)
 
 
@@ -211,14 +213,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.55.0
+--------------
+* added segmentation module
+
 Version 0.54.0
 --------------
 * added audeering public age and gender model embeddings and age and gender predictions
 
 Version 0.53.0
 --------------
 * added file checks: size in bytes and voice activity detection with silero
```

### Comparing `nkululeko-0.54.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.55.0/nkululeko.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 nkululeko/plots.py
 nkululeko/randomsplicer.py
 nkululeko/randomsplicing.py
 nkululeko/reporter.py
 nkululeko/result.py
 nkululeko/runmanager.py
 nkululeko/scaler.py
+nkululeko/segment.py
 nkululeko/syllable_nuclei.py
 nkululeko/test.py
 nkululeko/test_predictor.py
 nkululeko/util.py
 nkululeko.egg-info/PKG-INFO
 nkululeko.egg-info/SOURCES.txt
 nkululeko.egg-info/dependency_links.txt
```

### Comparing `nkululeko-0.54.0/setup.cfg` & `nkululeko-0.55.0/setup.cfg`

 * *Files identical despite different names*

