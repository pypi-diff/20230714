# Comparing `tmp/holisticai-0.5.0.tar.gz` & `tmp/holisticai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holisticai-0.5.0.tar", max compression
+gzip compressed data, was "holisticai-0.6.0.tar", max compression
```

## Comparing `holisticai-0.5.0.tar` & `holisticai-0.6.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0    11357 2023-06-27 20:41:50.394914 holisticai-0.5.0/LICENSE
--rw-r--r--   0        0        0      808 2023-06-27 20:41:50.394914 holisticai-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/__init__.py
--rw-r--r--   0        0        0      159 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/__init__.py
--rw-r--r--   0        0        0     3378 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/__init__.py
--rw-r--r--   0        0        0    28027 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_classification.py
--rw-r--r--   0        0        0    20317 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_clustering.py
--rw-r--r--   0        0        0    27996 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_multiclass.py
--rw-r--r--   0        0        0    41982 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_recommender.py
--rw-r--r--   0        0        0    30239 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_regression.py
--rw-r--r--   0        0        0     2212 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/__init__.py
--rw-r--r--   0        0        0     5662 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py
--rw-r--r--   0        0        0    10434 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py
--rw-r--r--   0        0        0     2149 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py
--rw-r--r--   0        0        0     1365 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py
--rw-r--r--   0        0        0     7801 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py
--rw-r--r--   0        0        0     2166 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py
--rw-r--r--   0        0        0     1977 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py
--rw-r--r--   0        0        0    14757 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py
--rw-r--r--   0        0        0       63 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_base.py
--rw-r--r--   0        0        0     8244 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py
--rw-r--r--   0        0        0     2832 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py
--rw-r--r--   0        0        0      140 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/__init__.py
--rw-r--r--   0        0        0       63 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_base.py
--rw-r--r--   0        0        0     8117 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py
--rw-r--r--   0        0        0     3093 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py
--rw-r--r--   0        0        0     1487 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/__init__.py
--rw-r--r--   0        0        0      740 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py
--rw-r--r--   0        0        0     2088 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py
--rw-r--r--   0        0        0     6067 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py
--rw-r--r--   0        0        0     7278 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py
--rw-r--r--   0        0        0       66 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/__init__.py
--rw-r--r--   0        0        0      475 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_conventions.py
--rw-r--r--   0        0        0     2381 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py
--rw-r--r--   0        0        0     2225 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py
--rw-r--r--   0        0        0    10288 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py
--rw-r--r--   0        0        0      906 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py
--rw-r--r--   0        0        0     4433 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py
--rw-r--r--   0        0        0     1435 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py
--rw-r--r--   0        0        0     7834 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py
--rw-r--r--   0        0        0     9599 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py
--rw-r--r--   0        0        0     6923 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py
--rw-r--r--   0        0        0    13843 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py
--rw-r--r--   0        0        0     4152 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py
--rw-r--r--   0        0        0     5017 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py
--rw-r--r--   0        0        0     2821 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py
--rw-r--r--   0        0        0    11078 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py
--rw-r--r--   0        0        0     3473 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py
--rw-r--r--   0        0        0     5213 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py
--rw-r--r--   0        0        0     1680 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py
--rw-r--r--   0        0        0     4772 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py
--rw-r--r--   0        0        0     3341 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py
--rw-r--r--   0        0        0     5644 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py
--rw-r--r--   0        0        0     6894 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py
--rw-r--r--   0        0        0     3231 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py
--rw-r--r--   0        0        0      559 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py
--rw-r--r--   0        0        0     1853 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py
--rw-r--r--   0        0        0     3541 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py
--rw-r--r--   0        0        0     9437 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py
--rw-r--r--   0        0        0     4493 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py
--rw-r--r--   0        0        0     2950 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py
--rw-r--r--   0        0        0     5287 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py
--rw-r--r--   0        0        0      614 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py
--rw-r--r--   0        0        0     3432 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py
--rw-r--r--   0        0        0     3952 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py
--rw-r--r--   0        0        0     3456 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py
--rw-r--r--   0        0        0     3437 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py
--rw-r--r--   0        0        0     3884 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py
--rw-r--r--   0        0        0     4088 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py
--rw-r--r--   0        0        0     6557 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py
--rw-r--r--   0        0        0     2217 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py
--rw-r--r--   0        0        0     2254 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py
--rw-r--r--   0        0        0     2231 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py
--rw-r--r--   0        0        0     2097 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py
--rw-r--r--   0        0        0     5463 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py
--rw-r--r--   0        0        0      828 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py
--rw-r--r--   0        0        0     4912 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py
--rw-r--r--   0        0        0     3457 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py
--rw-r--r--   0        0        0     3101 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py
--rw-r--r--   0        0        0     4954 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py
--rw-r--r--   0        0        0     1223 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/__init__.py
--rw-r--r--   0        0        0     8950 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py
--rw-r--r--   0        0        0     9796 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py
--rw-r--r--   0        0        0     7433 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py
--rw-r--r--   0        0        0     6954 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py
--rw-r--r--   0        0        0     4006 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py
--rw-r--r--   0        0        0     9322 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py
--rw-r--r--   0        0        0     6784 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py
--rw-r--r--   0        0        0     1963 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py
--rw-r--r--   0        0        0     2220 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py
--rw-r--r--   0        0        0     7114 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py
--rw-r--r--   0        0        0     3690 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py
--rw-r--r--   0        0        0     2278 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py
--rw-r--r--   0        0        0     2481 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py
--rw-r--r--   0        0        0     6238 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py
--rw-r--r--   0        0        0     3712 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py
--rw-r--r--   0        0        0      868 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py
--rw-r--r--   0        0        0     6369 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py
--rw-r--r--   0        0        0     5421 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py
--rw-r--r--   0        0        0     4286 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py
--rw-r--r--   0        0        0     3570 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py
--rw-r--r--   0        0        0     4032 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py
--rw-r--r--   0        0        0     1668 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py
--rw-r--r--   0        0        0     5413 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py
--rw-r--r--   0        0        0     2791 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py
--rw-r--r--   0        0        0     4968 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py
--rw-r--r--   0        0        0      640 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py
--rw-r--r--   0        0        0     5751 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py
--rw-r--r--   0        0        0     1314 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py
--rw-r--r--   0        0        0     1294 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py
--rw-r--r--   0        0        0     3844 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py
--rw-r--r--   0        0        0    10585 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py
--rw-r--r--   0        0        0     2177 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py
--rw-r--r--   0        0        0     3599 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py
--rw-r--r--   0        0        0      578 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/__init__.py
--rw-r--r--   0        0        0     3873 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py
--rw-r--r--   0        0        0     2674 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py
--rw-r--r--   0        0        0     3914 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py
--rw-r--r--   0        0        0     7337 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py
--rw-r--r--   0        0        0     3813 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/reweighing.py
--rw-r--r--   0        0        0     1343 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/__init__.py
--rw-r--r--   0        0        0     2157 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_classification_plots.py
--rw-r--r--   0        0        0     8449 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_exploratory_plots.py
--rw-r--r--   0        0        0    11349 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_multiclass_plots.py
--rw-r--r--   0        0        0     8066 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_recommender_plots.py
--rw-r--r--   0        0        0    14148 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_regression_plots.py
--rw-r--r--   0        0        0      333 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/__init__.py
--rw-r--r--   0        0        0    13961 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/_dataloaders.py
--rw-r--r--   0        0        0      951 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/synthetic/recruitment.py
--rw-r--r--   0        0        0      966 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/synthetic/user_feedback.py
--rw-r--r--   0        0        0    11570 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/efficacy/metrics.py
--rw-r--r--   0        0        0       54 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/__init__.py
--rw-r--r--   0        0        0     5952 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/_pipeline.py
--rw-r--r--   0        0        0     6559 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/_pipeline_helper.py
--rw-r--r--   0        0        0     3134 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/handlers/_estimator.py
--rw-r--r--   0        0        0     1821 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/handlers/_pipeline_params.py
--rw-r--r--   0        0        0     4816 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/handlers/_utransformers.py
--rw-r--r--   0        0        0      435 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/__init__.py
--rw-r--r--   0        0        0     5103 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_formatting.py
--rw-r--r--   0        0        0     1353 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_plotting.py
--rw-r--r--   0        0        0     5755 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_recommender_tools.py
--rw-r--r--   0        0        0    13794 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_validation.py
--rw-r--r--   0        0        0      100 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/__init__.py
--rw-r--r--   0        0        0     1908 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/_kcenters.py
--rw-r--r--   0        0        0    14757 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/_kmedoids.py
--rw-r--r--   0        0        0      549 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/_utils.py
--rw-r--r--   0        0        0      813 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/recommender/_rsbase.py
--rw-r--r--   0        0        0     3157 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/recommender/item_selection/selectors.py
--rw-r--r--   0        0        0     1321 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py
--rw-r--r--   0        0        0       68 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/optimizers/__init__.py
--rw-r--r--   0        0        0    15852 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/optimizers/_genetic_algorithm.py
--rw-r--r--   0        0        0     4484 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/_transformer_base.py
--rw-r--r--   0        0        0      499 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/__init__.py
--rw-r--r--   0        0        0     1049 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_group_utils.py
--rw-r--r--   0        0        0     1243 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_inprocessing.py
--rw-r--r--   0        0        0     2137 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_postprocessing.py
--rw-r--r--   0        0        0     1346 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_preprocessing.py
--rw-r--r--   0        0        0      699 2023-06-27 20:41:50.514913 holisticai-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 holisticai-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 21:31:48.801112 holisticai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1330 2023-07-14 21:31:48.801112 holisticai-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/__init__.py
+-rw-r--r--   0        0        0     3378 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/metrics/__init__.py
+-rw-r--r--   0        0        0    28027 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/metrics/_classification.py
+-rw-r--r--   0        0        0    20317 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/metrics/_clustering.py
+-rw-r--r--   0        0        0    27996 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/metrics/_multiclass.py
+-rw-r--r--   0        0        0    41982 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/metrics/_recommender.py
+-rw-r--r--   0        0        0    30239 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/metrics/_regression.py
+-rw-r--r--   0        0        0     2212 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/__init__.py
+-rw-r--r--   0        0        0     5662 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py
+-rw-r--r--   0        0        0    10434 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py
+-rw-r--r--   0        0        0     2149 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py
+-rw-r--r--   0        0        0     1365 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py
+-rw-r--r--   0        0        0     7801 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py
+-rw-r--r--   0        0        0     2166 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py
+-rw-r--r--   0        0        0     1977 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py
+-rw-r--r--   0        0        0    14757 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py
+-rw-r--r--   0        0        0       63 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_base.py
+-rw-r--r--   0        0        0     8244 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py
+-rw-r--r--   0        0        0     2832 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py
+-rw-r--r--   0        0        0      140 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_base.py
+-rw-r--r--   0        0        0     8117 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py
+-rw-r--r--   0        0        0     3093 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py
+-rw-r--r--   0        0        0     1487 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py
+-rw-r--r--   0        0        0     2088 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py
+-rw-r--r--   0        0        0     6067 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py
+-rw-r--r--   0        0        0     7278 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py
+-rw-r--r--   0        0        0       66 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/__init__.py
+-rw-r--r--   0        0        0      475 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/_conventions.py
+-rw-r--r--   0        0        0     2381 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py
+-rw-r--r--   0        0        0     2225 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py
+-rw-r--r--   0        0        0    10288 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py
+-rw-r--r--   0        0        0      906 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py
+-rw-r--r--   0        0        0     4433 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py
+-rw-r--r--   0        0        0     1435 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py
+-rw-r--r--   0        0        0     7834 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py
+-rw-r--r--   0        0        0     9599 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py
+-rw-r--r--   0        0        0     6923 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py
+-rw-r--r--   0        0        0    13843 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py
+-rw-r--r--   0        0        0     4152 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py
+-rw-r--r--   0        0        0     5017 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py
+-rw-r--r--   0        0        0     2821 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py
+-rw-r--r--   0        0        0    11078 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py
+-rw-r--r--   0        0        0     3473 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py
+-rw-r--r--   0        0        0     5213 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py
+-rw-r--r--   0        0        0     1680 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py
+-rw-r--r--   0        0        0     4772 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py
+-rw-r--r--   0        0        0     3341 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py
+-rw-r--r--   0        0        0     5644 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py
+-rw-r--r--   0        0        0     6894 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py
+-rw-r--r--   0        0        0     3231 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py
+-rw-r--r--   0        0        0      559 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py
+-rw-r--r--   0        0        0     1853 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py
+-rw-r--r--   0        0        0     3541 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py
+-rw-r--r--   0        0        0     9437 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py
+-rw-r--r--   0        0        0     4493 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py
+-rw-r--r--   0        0        0     2950 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py
+-rw-r--r--   0        0        0     5287 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py
+-rw-r--r--   0        0        0      614 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py
+-rw-r--r--   0        0        0     3432 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py
+-rw-r--r--   0        0        0     3952 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py
+-rw-r--r--   0        0        0     3456 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py
+-rw-r--r--   0        0        0     3437 2023-07-14 21:31:48.929121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py
+-rw-r--r--   0        0        0     3884 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py
+-rw-r--r--   0        0        0     4088 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py
+-rw-r--r--   0        0        0     6557 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py
+-rw-r--r--   0        0        0     2217 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py
+-rw-r--r--   0        0        0     2254 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py
+-rw-r--r--   0        0        0     2231 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py
+-rw-r--r--   0        0        0     2097 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py
+-rw-r--r--   0        0        0     5463 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py
+-rw-r--r--   0        0        0      828 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py
+-rw-r--r--   0        0        0     4968 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py
+-rw-r--r--   0        0        0     3457 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py
+-rw-r--r--   0        0        0     3101 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py
+-rw-r--r--   0        0        0     4954 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py
+-rw-r--r--   0        0        0     1223 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/__init__.py
+-rw-r--r--   0        0        0     8950 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py
+-rw-r--r--   0        0        0     9796 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py
+-rw-r--r--   0        0        0     7433 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py
+-rw-r--r--   0        0        0     6954 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py
+-rw-r--r--   0        0        0     4006 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py
+-rw-r--r--   0        0        0     9322 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py
+-rw-r--r--   0        0        0     6784 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py
+-rw-r--r--   0        0        0     1963 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py
+-rw-r--r--   0        0        0     2220 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py
+-rw-r--r--   0        0        0     7114 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py
+-rw-r--r--   0        0        0     3690 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py
+-rw-r--r--   0        0        0     2278 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py
+-rw-r--r--   0        0        0     2481 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py
+-rw-r--r--   0        0        0     6238 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py
+-rw-r--r--   0        0        0     3712 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py
+-rw-r--r--   0        0        0      868 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py
+-rw-r--r--   0        0        0     6369 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py
+-rw-r--r--   0        0        0     5421 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py
+-rw-r--r--   0        0        0     4286 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py
+-rw-r--r--   0        0        0     3570 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py
+-rw-r--r--   0        0        0     4032 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py
+-rw-r--r--   0        0        0     1668 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py
+-rw-r--r--   0        0        0     5413 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py
+-rw-r--r--   0        0        0     2791 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py
+-rw-r--r--   0        0        0     4968 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py
+-rw-r--r--   0        0        0      640 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py
+-rw-r--r--   0        0        0     5751 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py
+-rw-r--r--   0        0        0     1314 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py
+-rw-r--r--   0        0        0     1294 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py
+-rw-r--r--   0        0        0     3844 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py
+-rw-r--r--   0        0        0    10585 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py
+-rw-r--r--   0        0        0     2344 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py
+-rw-r--r--   0        0        0     3599 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py
+-rw-r--r--   0        0        0      578 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3873 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py
+-rw-r--r--   0        0        0     2674 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py
+-rw-r--r--   0        0        0     3914 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py
+-rw-r--r--   0        0        0     7337 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py
+-rw-r--r--   0        0        0     3813 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/reweighing.py
+-rw-r--r--   0        0        0     1343 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/plots/__init__.py
+-rw-r--r--   0        0        0     2157 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/plots/_bias_classification_plots.py
+-rw-r--r--   0        0        0     8449 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/plots/_bias_exploratory_plots.py
+-rw-r--r--   0        0        0    11349 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/plots/_bias_multiclass_plots.py
+-rw-r--r--   0        0        0     8066 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/plots/_bias_recommender_plots.py
+-rw-r--r--   0        0        0    14148 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/bias/plots/_bias_regression_plots.py
+-rw-r--r--   0        0        0      333 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/datasets/__init__.py
+-rw-r--r--   0        0        0    13961 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/datasets/_dataloaders.py
+-rw-r--r--   0        0        0      951 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/datasets/synthetic/recruitment.py
+-rw-r--r--   0        0        0      966 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/datasets/synthetic/user_feedback.py
+-rw-r--r--   0        0        0    11570 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/efficacy/metrics.py
+-rw-r--r--   0        0        0       54 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5952 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/pipeline/_pipeline.py
+-rw-r--r--   0        0        0     6559 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/pipeline/_pipeline_helper.py
+-rw-r--r--   0        0        0     3134 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/pipeline/handlers/_estimator.py
+-rw-r--r--   0        0        0     1821 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/pipeline/handlers/_pipeline_params.py
+-rw-r--r--   0        0        0     4816 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/pipeline/handlers/_utransformers.py
+-rw-r--r--   0        0        0      435 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/__init__.py
+-rw-r--r--   0        0        0     5103 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/_formatting.py
+-rw-r--r--   0        0        0     1353 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/_plotting.py
+-rw-r--r--   0        0        0     5755 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/_recommender_tools.py
+-rw-r--r--   0        0        0    13794 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/_validation.py
+-rw-r--r--   0        0        0      100 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/cluster/__init__.py
+-rw-r--r--   0        0        0     1908 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/cluster/_kcenters.py
+-rw-r--r--   0        0        0    14757 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/cluster/_kmedoids.py
+-rw-r--r--   0        0        0      549 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/cluster/_utils.py
+-rw-r--r--   0        0        0      813 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/recommender/_rsbase.py
+-rw-r--r--   0        0        0     3157 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/recommender/item_selection/selectors.py
+-rw-r--r--   0        0        0     1321 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py
+-rw-r--r--   0        0        0       68 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/optimizers/__init__.py
+-rw-r--r--   0        0        0    15852 2023-07-14 21:31:48.933121 holisticai-0.6.0/holisticai/utils/optimizers/_genetic_algorithm.py
+-rw-r--r--   0        0        0     4484 2023-07-14 21:31:48.937121 holisticai-0.6.0/holisticai/utils/transformers/_transformer_base.py
+-rw-r--r--   0        0        0      499 2023-07-14 21:31:48.937121 holisticai-0.6.0/holisticai/utils/transformers/bias/__init__.py
+-rw-r--r--   0        0        0     1049 2023-07-14 21:31:48.937121 holisticai-0.6.0/holisticai/utils/transformers/bias/_group_utils.py
+-rw-r--r--   0        0        0     1243 2023-07-14 21:31:48.937121 holisticai-0.6.0/holisticai/utils/transformers/bias/_inprocessing.py
+-rw-r--r--   0        0        0     2137 2023-07-14 21:31:48.937121 holisticai-0.6.0/holisticai/utils/transformers/bias/_postprocessing.py
+-rw-r--r--   0        0        0     1346 2023-07-14 21:31:48.937121 holisticai-0.6.0/holisticai/utils/transformers/bias/_preprocessing.py
+-rw-r--r--   0        0        0      871 2023-07-14 21:31:48.937121 holisticai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 holisticai-0.6.0/PKG-INFO
```

### Comparing `holisticai-0.5.0/LICENSE` & `holisticai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/metrics/__init__.py` & `holisticai-0.6.0/holisticai/bias/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/metrics/_classification.py` & `holisticai-0.6.0/holisticai/bias/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/metrics/_clustering.py` & `holisticai-0.6.0/holisticai/bias/metrics/_clustering.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/metrics/_multiclass.py` & `holisticai-0.6.0/holisticai/bias/metrics/_multiclass.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/metrics/_recommender.py` & `holisticai-0.6.0/holisticai/bias/metrics/_recommender.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/metrics/_regression.py` & `holisticai-0.6.0/holisticai/bias/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/__init__.py` & `holisticai-0.6.0/holisticai/bias/mitigation/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py` & `holisticai-0.6.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/__init__.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         x_squared_norms = x_squared_norms[init_indices]
         n_samples = X.shape[0]
 
     if isinstance(init, str) and init == "k-means++":
         centers, _ = _kmeans_plusplus(
             X,
             n_clusters,
+            sample_weight=np.ones(shape=(X.shape[0],)),
             random_state=random_state,
             x_squared_norms=x_squared_norms,
         )
     elif isinstance(init, str) and init == "random":
         seeds = random_state.permutation(n_samples)[:n_clusters]
         centers = X[seeds]
     elif _is_arraylike_not_scalar(init):
```

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/__init__.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,22 +34,23 @@
         noise = self.eps * np.random.randn(len(y_pred)).squeeze()
         self.YL = y_pred + noise
 
         self.minY = np.min(self.YL)
         self.maxY = np.max(self.YL)
 
     def _optimize_ts(self, yt, i1, i2, n1, n2):
-        dist_best = np.inf
-        for t in np.linspace(self.minY, self.maxY, 100):
-            tmp1 = np.sum(self.YL[self.SL == self.group_values[i1]] < t) / n1
-            tmp2 = np.sum(self.YL[self.SL == self.group_values[i2]] < yt) / n2
-            dist = np.abs(tmp1 - tmp2)
-            if dist_best > dist:
-                dist_best = dist
-                ts = t
+        mask1 = self.SL == self.group_values[i1]
+        mask2 = self.SL == self.group_values[i2]
+        yl_masked2 = self.YL[mask2]
+        tmp2 = np.sum(yl_masked2 < yt) / n2
+        yl_masked1 = self.YL[mask1]
+        t_values = np.linspace(self.minY, self.maxY, 100)
+        tmp1 = np.sum(yl_masked1[:, None] < t_values, axis=0) / n1
+        dist = np.abs(tmp1 - tmp2)
+        ts = t_values[np.argmin(dist)]
         return ts
 
     def _update_yt(self, yt, group):
         if group == self.group_values[self.im]:
             ts = self._optimize_ts(yt, self.iM, self.im, self.nM, self.nm)
             yf = self.p * yt + (1 - self.p) * ts
 
@@ -58,9 +59,14 @@
             yf = self.q * yt + (1 - self.q) * ts
         return yf
 
     def transform(self, y_pred: np.ndarray, sensitive_groups: np.ndarray):
         ST = self.sens_groups.transform(sensitive_groups, convert_numeric=True)
         noise = self.eps * np.random.randn(len(y_pred)).squeeze()
         YT = y_pred + noise
+        import time
+
+        tic = time.time()
         YF = np.array([self._update_yt(yt, st) for yt, st in zip(YT, ST)])
+        toc = time.time()
+        print("Time taken: {}".format(toc - tic))
         return YF
```

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/__init__.py` & `holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py` & `holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py` & `holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py` & `holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py` & `holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/reweighing.py` & `holisticai-0.6.0/holisticai/bias/mitigation/preprocessing/reweighing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/plots/__init__.py` & `holisticai-0.6.0/holisticai/bias/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/plots/_bias_classification_plots.py` & `holisticai-0.6.0/holisticai/bias/plots/_bias_classification_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/plots/_bias_exploratory_plots.py` & `holisticai-0.6.0/holisticai/bias/plots/_bias_exploratory_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/plots/_bias_multiclass_plots.py` & `holisticai-0.6.0/holisticai/bias/plots/_bias_multiclass_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/plots/_bias_recommender_plots.py` & `holisticai-0.6.0/holisticai/bias/plots/_bias_recommender_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/bias/plots/_bias_regression_plots.py` & `holisticai-0.6.0/holisticai/bias/plots/_bias_regression_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/datasets/_dataloaders.py` & `holisticai-0.6.0/holisticai/datasets/_dataloaders.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/datasets/synthetic/recruitment.py` & `holisticai-0.6.0/holisticai/datasets/synthetic/recruitment.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/datasets/synthetic/user_feedback.py` & `holisticai-0.6.0/holisticai/datasets/synthetic/user_feedback.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/efficacy/metrics.py` & `holisticai-0.6.0/holisticai/efficacy/metrics.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/pipeline/_pipeline.py` & `holisticai-0.6.0/holisticai/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/pipeline/_pipeline_helper.py` & `holisticai-0.6.0/holisticai/pipeline/_pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/pipeline/handlers/_estimator.py` & `holisticai-0.6.0/holisticai/pipeline/handlers/_estimator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/pipeline/handlers/_pipeline_params.py` & `holisticai-0.6.0/holisticai/pipeline/handlers/_pipeline_params.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/pipeline/handlers/_utransformers.py` & `holisticai-0.6.0/holisticai/pipeline/handlers/_utransformers.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/_formatting.py` & `holisticai-0.6.0/holisticai/utils/_formatting.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/_plotting.py` & `holisticai-0.6.0/holisticai/utils/_plotting.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/_recommender_tools.py` & `holisticai-0.6.0/holisticai/utils/_recommender_tools.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/_validation.py` & `holisticai-0.6.0/holisticai/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/models/cluster/_kcenters.py` & `holisticai-0.6.0/holisticai/utils/models/cluster/_kcenters.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/models/cluster/_kmedoids.py` & `holisticai-0.6.0/holisticai/utils/models/cluster/_kmedoids.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/models/cluster/_utils.py` & `holisticai-0.6.0/holisticai/utils/models/cluster/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/models/recommender/_rsbase.py` & `holisticai-0.6.0/holisticai/utils/models/recommender/_rsbase.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/models/recommender/item_selection/selectors.py` & `holisticai-0.6.0/holisticai/utils/models/recommender/item_selection/selectors.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py` & `holisticai-0.6.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/optimizers/_genetic_algorithm.py` & `holisticai-0.6.0/holisticai/utils/optimizers/_genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/transformers/_transformer_base.py` & `holisticai-0.6.0/holisticai/utils/transformers/_transformer_base.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/transformers/bias/_group_utils.py` & `holisticai-0.6.0/holisticai/utils/transformers/bias/_group_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/transformers/bias/_inprocessing.py` & `holisticai-0.6.0/holisticai/utils/transformers/bias/_inprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/transformers/bias/_postprocessing.py` & `holisticai-0.6.0/holisticai/utils/transformers/bias/_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/holisticai/utils/transformers/bias/_preprocessing.py` & `holisticai-0.6.0/holisticai/utils/transformers/bias/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.5.0/pyproject.toml` & `holisticai-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [tool.commitizen]
-version = "0.5.0"
+version = "0.6.0"
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
 
 [tool.poetry]
 name = "holisticai"
-version = "0.5.0"
+version = "0.6.0"
 description = "Holistic AI Library"
 authors = ["Research Team"]
 maintainers = ["Research Team <researchteam@holisticai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
 scikit-learn = ">=1.0.2"
-seaborn = ">=0.11.2"
-tqdm = "^4.64.1"
-cvxpy = {extras = ["cbc"], version = "^1.3.0"}
-cvxopt = "^1.3.0"
+
+tqdm = {version=">=4.64.1" , optional = true}
+cvxpy = {extras=["cbc"], version=">1.3.0" , optional = true}
+cvxopt = {version=">=1.3.0" , optional = true}
+seaborn = {version=">=0.11.2" , optional = true}
+
+[tool.poetry.extras]
+methods = ["tqdm", "cvxpy", "cvxopt", "seaborn"]
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
 pytest = "^7.1.3"
 commitizen = "^2.40.0"
```

### Comparing `holisticai-0.5.0/PKG-INFO` & `holisticai-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: holisticai
-Version: 0.5.0
+Version: 0.6.0
 Summary: Holistic AI Library
 Author: Research Team
 Maintainer: Research Team
 Maintainer-email: researchteam@holisticai.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cvxopt (>=1.3.0,<2.0.0)
-Requires-Dist: cvxpy[cbc] (>=1.3.0,<2.0.0)
+Provides-Extra: methods
+Requires-Dist: cvxopt (>=1.3.0) ; extra == "methods"
+Requires-Dist: cvxpy[cbc] (>1.3.0) ; extra == "methods"
 Requires-Dist: scikit-learn (>=1.0.2)
-Requires-Dist: seaborn (>=0.11.2)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: seaborn (>=0.11.2) ; extra == "methods"
+Requires-Dist: tqdm (>=4.64.1) ; extra == "methods"
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 <img src="docs/holistic_ai.png" width="100">
 <br>Holistic AI
 </h1>
 
@@ -28,14 +29,30 @@
 Currently, the library offers a set of techniques to easily measure and mitigate Bias across numerous tasks. In the future, it will be extended to include tools for Efficacy, Robustness, Privacy and Explainability as well. This will allow a holistic assessment of AI systems.  
 
 - Documentation: https://holistic-ai.readthedocs.io/en/latest/
 - Tutorials: https://github.com/holistic-ai/holisticai/tree/main/tutorials
 - Source code: https://github.com/holistic-ai/holisticai/tree/main
 - Holistic Ai website: https://holisticai.com
 
-## Installation
 
-Install the library with:
+# Installation:
+For metrics, you can use the default installation:
+
+```bash
+pip install holisticai
+```
+For bias visualization and mitigation, you need additional dependencies. You can install them with:
+ ```bash
+pip install holisticai[methods]
+```
+## Troubleshooting
+on **macOS** could be necessary some packages before install holisticai library:
 ```bash
-    pip install holisticai
+brew install cbc pkg-config
+python -m pip install cylp
+brew install cmake
 ```
 
+## Contributing
+
+We welcome contributions to the Holistic AI library. If you are interested in contributing, please refer to our [contributing guide](CONTRIBUTING.md).
+
```

