# Comparing `tmp/nzpyida-0.9.1.tar.gz` & `tmp/nzpyida-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.9.1.tar", last modified: Wed Jul 12 14:04:22 2023, max compression
+gzip compressed data, was "nzpyida-0.9.2.tar", last modified: Fri Jul 14 14:36:08 2023, max compression
```

## Comparing `nzpyida-0.9.1.tar` & `nzpyida-0.9.2.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.265563 nzpyida-0.9.1/
--rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9.1/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9.1/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.9.1/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-12 14:04:22.265647 nzpyida-0.9.1/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9.1/README.md
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.232416 nzpyida-0.9.1/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9.1/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.235826 nzpyida-0.9.1/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    11955 2023-07-12 13:59:27.000000 nzpyida-0.9.1/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/geoFrame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/geoSeries.rst
--rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1557 2023-07-12 13:55:25.000000 nzpyida-0.9.1/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9.1/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9.1/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.239665 nzpyida-0.9.1/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.9.1/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.242507 nzpyida-0.9.1/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.245172 nzpyida-0.9.1/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.245362 nzpyida-0.9.1/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.246338 nzpyida-0.9.1/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9.1/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9.1/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.247272 nzpyida-0.9.1/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.250972 nzpyida-0.9.1/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)    29001 2023-06-20 14:25:25.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/bayesian_networks.py
--rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     8440 2023-05-29 14:08:02.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/glm.py
--rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.255254 nzpyida-0.9.1/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     3588 2023-07-06 15:07:05.000000 nzpyida-0.9.1/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-07-06 15:02:50.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     6678 2023-06-20 14:25:25.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_bayesian_networks.py
--rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2067 2023-05-29 14:08:02.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_cross_validation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_glm.py
--rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     3041 2023-05-29 14:08:02.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.255970 nzpyida-0.9.1/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)    10990 2023-07-12 13:55:25.000000 nzpyida-0.9.1/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5176 2023-07-12 13:55:25.000000 nzpyida-0.9.1/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.9.1/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.258291 nzpyida-0.9.1/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.9.1/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.260262 nzpyida-0.9.1/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-25 14:47:30.000000 nzpyida-0.9.1/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9.1/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-07-06 15:02:38.000000 nzpyida-0.9.1/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.265380 nzpyida-0.9.1/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.9.1/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.9.1/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.9.1/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.9.1/nzpyida/tests/test_geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.9.1/nzpyida/tests/test_geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.9.1/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-12 14:04:22.240427 nzpyida-0.9.1/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-12 14:04:22.000000 nzpyida-0.9.1/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4875 2023-07-12 14:04:22.000000 nzpyida-0.9.1/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-07-12 14:04:22.000000 nzpyida-0.9.1/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-07-12 14:04:22.000000 nzpyida-0.9.1/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-07-12 14:04:22.000000 nzpyida-0.9.1/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      177 2023-07-12 14:04:22.266021 nzpyida-0.9.1/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     3318 2023-07-12 13:59:27.000000 nzpyida-0.9.1/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.864126 nzpyida-0.9.2/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9.2/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9.2/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.9.2/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-14 14:36:08.864207 nzpyida-0.9.2/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9.2/README.md
+-rw-r--r--   0 mpl        (501) staff       (20)        5 2023-07-14 11:52:20.000000 nzpyida-0.9.2/VERSION
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.825519 nzpyida-0.9.2/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9.2/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.829037 nzpyida-0.9.2/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    12029 2023-07-14 11:58:59.000000 nzpyida-0.9.2/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/geoFrame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/geoSeries.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1557 2023-07-12 13:55:25.000000 nzpyida-0.9.2/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9.2/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9.2/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.837618 nzpyida-0.9.2/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.9.2/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.841570 nzpyida-0.9.2/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.843278 nzpyida-0.9.2/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.843481 nzpyida-0.9.2/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.845094 nzpyida-0.9.2/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9.2/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9.2/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.845848 nzpyida-0.9.2/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.849957 nzpyida-0.9.2/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)    29001 2023-06-20 14:25:25.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8440 2023-07-14 08:41:28.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-07-13 09:52:03.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.854990 nzpyida-0.9.2/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     3588 2023-07-06 15:07:05.000000 nzpyida-0.9.2/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-07-06 15:02:50.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6678 2023-06-20 14:25:25.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2067 2023-05-29 14:08:02.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_cross_validation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3041 2023-05-29 14:08:02.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.855778 nzpyida-0.9.2/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10667 2023-07-14 08:34:35.000000 nzpyida-0.9.2/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10990 2023-07-12 13:55:25.000000 nzpyida-0.9.2/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5176 2023-07-12 13:55:25.000000 nzpyida-0.9.2/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.9.2/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.857667 nzpyida-0.9.2/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    90288 2023-07-14 10:27:18.000000 nzpyida-0.9.2/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.859285 nzpyida-0.9.2/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-07-14 08:41:35.000000 nzpyida-0.9.2/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9.2/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-07-06 15:02:38.000000 nzpyida-0.9.2/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.863959 nzpyida-0.9.2/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.9.2/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.9.2/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.9.2/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.9.2/nzpyida/tests/test_geoFrame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.9.2/nzpyida/tests/test_geoSeries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.9.2/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-14 14:36:08.838754 nzpyida-0.9.2/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4883 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-07-14 14:36:08.000000 nzpyida-0.9.2/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      213 2023-07-14 14:36:08.864483 nzpyida-0.9.2/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3300 2023-07-14 11:55:18.000000 nzpyida-0.9.2/setup.py
```

### Comparing `nzpyida-0.9.1/LICENSE.txt` & `nzpyida-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/PKG-INFO` & `nzpyida-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.9.1
+Version: 0.9.2
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.9.1/README.md` & `nzpyida-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/.DS_Store` & `nzpyida-0.9.2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/Makefile` & `nzpyida-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/make.bat` & `nzpyida-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/base.rst` & `nzpyida-0.9.2/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/conf.py` & `nzpyida-0.9.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.pardir)
 basepath = os.path.dirname(__file__)
 filepath = os.path.abspath(os.path.join(basepath, "..", "..", "nzpyida"))
 sys.path.append(filepath)
+
+with open(os.path.join(basepath, '..', '..', 'VERSION')) as f:
+    ver = f.read()
+
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -67,17 +71,17 @@
 author = u''
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u'0.9.1'
+version = ver
 # The full version, including alpha/beta/rc tags.
-release = u'0.9.1'
+release = ver
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'english'
```

### Comparing `nzpyida-0.9.1/docs/source/frame.rst` & `nzpyida-0.9.2/docs/source/frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/geoFrame.rst` & `nzpyida-0.9.2/docs/source/geoFrame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/geoSeries.rst` & `nzpyida-0.9.2/docs/source/geoSeries.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/geospatial.rst` & `nzpyida-0.9.2/docs/source/geospatial.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/ibm.png` & `nzpyida-0.9.2/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/index.rst` & `nzpyida-0.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/install.rst` & `nzpyida-0.9.2/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/kc.ico` & `nzpyida-0.9.2/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/legal.rst` & `nzpyida-0.9.2/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/predictive.rst` & `nzpyida-0.9.2/docs/source/predictive.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/start.rst` & `nzpyida-0.9.2/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/docs/source/utils.rst` & `nzpyida-0.9.2/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/__init__.py` & `nzpyida-0.9.2/nzpyida/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/__init__.py` & `nzpyida-0.9.2/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/apply.py` & `nzpyida-0.9.2/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.9.2/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.9.2/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.9.2/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.9.2/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/groupedapply.py` & `nzpyida-0.9.2/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/install.py` & `nzpyida-0.9.2/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/result_builder.py` & `nzpyida-0.9.2/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/shaper.py` & `nzpyida-0.9.2/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/tapply.py` & `nzpyida-0.9.2/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/tapply_class.py` & `nzpyida-0.9.2/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.9.2/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/aggregation.py` & `nzpyida-0.9.2/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/__init__.py` & `nzpyida-0.9.2/nzpyida/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.9.2/nzpyida/analytics/auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.9.2/nzpyida/analytics/exploration/distribution.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.9.2/nzpyida/analytics/exploration/relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/model_manager.py` & `nzpyida-0.9.2/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/bayesian_networks.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/bayesian_networks.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/classification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/glm.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/timeseries.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.9.2/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/conftest.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_bayesian_networks.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_bayesian_networks.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_cross_validation.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_glm.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_relation_identification.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_timeseries.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.9.2/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.9.2/nzpyida/analytics/transform/discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             the output table with dicretization bins
 
         Returns
         -------
         IdaDataFrame
             the data frame with discretization bins
         """
-        in_columns = ';'.join(in_df.columns)
+        in_columns = ';'.join(['"' + x + '"' for x in in_df.columns])
         params_dict = {
             'incolumn': in_columns,
             'outtabletype': 'table'
         }
         params_dict.update(self.params)
 
         return call_proc_df_in_out(proc=self.proc, in_df=in_df, params=params_dict,
```

### Comparing `nzpyida-0.9.1/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.9.2/nzpyida/analytics/transform/preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/analytics/utils.py` & `nzpyida-0.9.2/nzpyida/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/base.py` & `nzpyida-0.9.2/nzpyida/base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/exceptions.py` & `nzpyida-0.9.2/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/__init__.py` & `nzpyida-0.9.2/nzpyida/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.9.2/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/entropy.py` & `nzpyida-0.9.2/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.9.2/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/gini.py` & `nzpyida-0.9.2/nzpyida/feature_selection/gini.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.9.2/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/private.py` & `nzpyida-0.9.2/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/symmetric_uncertainty.py` & `nzpyida-0.9.2/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/feature_selection/tstats.py` & `nzpyida-0.9.2/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/filtering.py` & `nzpyida-0.9.2/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/frame.py` & `nzpyida-0.9.2/nzpyida/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1072,21 +1072,20 @@
                             column = self._get_numerical_columns()[0]
                         order = " ORDER BY \"" + column + "\" ASC"
                     else:
                         order = ''
             data = self.ida_query("SELECT * FROM %s %s LIMIT %s "%(name, order, nrow))
 
             if data.shape[0] != 0:
-                # otherwise column sort order is reverted
-                if not 'SELECT ' in name:
+                if isinstance(self, nzpyida.IdaSeries):
+                    data = data[self.columns[0]]
+                elif not 'SELECT ' in name:
                     columns = self.columns
                     data.columns = columns
 #                data = ibmdbpy.utils._convert_dtypes(self, data)
-                if isinstance(self, nzpyida.IdaSeries):
-                    data = pd.Series(data)
             return data
 
     # TODO : There is a warning in anaconda when there are missing values -> why ?
     @idadf_state
     def tail(self, nrow=5, sort=True):
         """
         Print the n last rows of the instance, n is set to 5 by default.
```

### Comparing `nzpyida-0.9.1/nzpyida/indexing.py` & `nzpyida-0.9.2/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/internals.py` & `nzpyida-0.9.2/nzpyida/internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/__init__.py` & `nzpyida-0.9.2/nzpyida/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/iris.py` & `nzpyida-0.9.2/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/iris.txt` & `nzpyida-0.9.2/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/swiss.py` & `nzpyida-0.9.2/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/swiss.txt` & `nzpyida-0.9.2/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/titanic.py` & `nzpyida-0.9.2/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sampledata/titanic.txt` & `nzpyida-0.9.2/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/series.py` & `nzpyida-0.9.2/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/sql.py` & `nzpyida-0.9.2/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/statistics.py` & `nzpyida-0.9.2/nzpyida/statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/conftest.py` & `nzpyida-0.9.2/nzpyida/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_aggregation.py` & `nzpyida-0.9.2/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_association_rules.py` & `nzpyida-0.9.2/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_base.py` & `nzpyida-0.9.2/nzpyida/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.9.2/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_base_private.py` & `nzpyida-0.9.2/nzpyida/tests/test_base_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.9.2/nzpyida/tests/test_base_table_manipulation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.9.2/nzpyida/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_filtering.py` & `nzpyida-0.9.2/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_frame.py` & `nzpyida-0.9.2/nzpyida/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.9.2/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_frame_private.py` & `nzpyida-0.9.2/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_geoFrame.py` & `nzpyida-0.9.2/nzpyida/tests/test_geoFrame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_geoSeries.py` & `nzpyida-0.9.2/nzpyida/tests/test_geoSeries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_indexing.py` & `nzpyida-0.9.2/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_internals.py` & `nzpyida-0.9.2/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_kmeans.py` & `nzpyida-0.9.2/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.9.2/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_series.py` & `nzpyida-0.9.2/nzpyida/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_sorting.py` & `nzpyida-0.9.2/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_statistics.py` & `nzpyida-0.9.2/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/tests/test_utils.py` & `nzpyida-0.9.2/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida/utils.py` & `nzpyida-0.9.2/nzpyida/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.1/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.9.2/nzpyida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.9.1
+Version: 0.9.2
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.9.1/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.9.2/nzpyida.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
+VERSION
 setup.cfg
 setup.py
 docs/.DS_Store
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/analytics.rst
```

### Comparing `nzpyida-0.9.1/setup.py` & `nzpyida-0.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -62,15 +62,14 @@
 
         'Topic :: Database',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
       ]
 
 setup(name='nzpyida',
-      version='0.9.1',
       install_requires=['pandas','numpy','future','six','pypyodbc','pyodbc', 'lazy', 'nzpy'],
 
       extras_require={
         'jdbc':['JayDeBeApi==1.*', 'Jpype1==0.6.3'],
         'test':['pytest', 'flaky==3.4.0'],
         'doc':['sphinx', 'ipython', 'numpydoc', 'sphinx_rtd_theme']
       },
```

