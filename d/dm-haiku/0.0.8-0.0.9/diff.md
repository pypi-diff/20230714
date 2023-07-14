# Comparing `tmp/dm-haiku-0.0.8.tar.gz` & `tmp/dm-haiku-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-haiku-0.0.8.tar", last modified: Wed Sep 21 14:11:08 2022, max compression
+gzip compressed data, was "dm-haiku-0.0.9.tar", last modified: Wed Nov 16 12:15:30 2022, max compression
```

## Comparing `dm-haiku-0.0.8.tar` & `dm-haiku-0.0.9.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17863 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16912 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/dm_haiku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17863 2022-09-21 14:11:08.000000 dm-haiku-0.0.8/dm_haiku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-09-21 14:11:08.000000 dm-haiku-0.0.8/dm_haiku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 14:11:08.000000 dm-haiku-0.0.8/dm_haiku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 14:11:08.000000 dm-haiku-0.0.8/dm_haiku.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-21 14:11:08.000000 dm-haiku-0.0.8/dm_haiku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-21 14:11:08.000000 dm-haiku-0.0.8/dm_haiku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7617 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/docs/ext/coverage_check.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/examples/imagenet/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/imagenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11100 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/imagenet/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    13269 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/imagenet/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/examples/impala/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/actor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/actor_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     5316 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/haiku_nets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7684 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/learner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/learner_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/run_catch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/impala/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/examples/rnn/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/rnn/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     6605 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/rnn/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.800982 dm-haiku-0.0.8/examples/transformer/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/transformer/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/transformer/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5406 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/examples/transformer/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.804982 dm-haiku-0.0.8/haiku/
--rw-r--r--   0 runner    (1001) docker     (121)     7832 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/haiku/_src/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/analytics.py
--rw-r--r--   0 runner    (1001) docker     (121)     6117 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    40131 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    28859 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12002 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8184 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/basic_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8580 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8676 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/batch_norm_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6022 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/bias.py
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/bias_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10504 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/config_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    32135 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/conv.py
--rw-r--r--   0 runner    (1001) docker     (121)    28811 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/conv_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10819 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    14051 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/data_structures_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/deferred.py
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/deferred_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13407 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)    12738 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/depthwise_conv_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13253 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/dot.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/dot_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7997 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/embed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/embed_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/eval_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/eval_shape_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9089 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)    13860 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/filtering_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8887 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/group_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)    10706 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/group_norm_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11827 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/initializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7869 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/initializers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/haiku/_src/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/check_tracer_leaks_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/checkpoint_generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    12749 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/descriptors_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/doctest_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/float64_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/half_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9614 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/hk_transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/jax2tf_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/jax_transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/jaxpr_info_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/numpy_inputs_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/rank_promotion_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/replaceable_funcs_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/shim_hk_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/summarise_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/to_dot_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/integration/typing_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21685 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/jaxpr_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     5014 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/jaxpr_info_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9998 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)     9359 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/layer_norm_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9999 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)    17843 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/layer_stack_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16467 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/lift.py
--rw-r--r--   0 runner    (1001) docker     (121)    19086 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/lift_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8721 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     7313 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/mixed_precision_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    29198 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/module.py
--rw-r--r--   0 runner    (1001) docker     (121)    32641 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/module_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7772 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/moving_averages.py
--rw-r--r--   0 runner    (1001) docker     (121)     9498 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/moving_averages_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11720 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/multi_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/multi_transform_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/haiku/_src/nets/
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5766 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/mlp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6920 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/mlp_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/mobilenetv1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/mobilenetv1_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21716 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     6714 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    14856 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/vqvae.py
--rw-r--r--   0 runner    (1001) docker     (121)     8055 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/nets/vqvae_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/pad.py
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/pad_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7420 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     9267 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/pool_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/random_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    28064 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/recurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)    19197 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/reshape.py
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/reshape_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/rms_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/rms_norm_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6752 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/spectral_norm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/spectral_norm_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    34846 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/stateful.py
--rw-r--r--   0 runner    (1001) docker     (121)    31146 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/stateful_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    15463 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/summarise.py
--rw-r--r--   0 runner    (1001) docker     (121)     8856 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/summarise_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7869 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/test_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    15584 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    21738 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/typing_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9172 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5781 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/_src/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/haiku/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/benchmarks/eval_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/benchmarks/init.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/data_structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/haiku/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/experimental/jaxpr_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/initializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/nets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/pad.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/haiku/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/requirements-jax.txt
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 14:11:08.812982 dm-haiku-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-09-21 14:10:58.000000 dm-haiku-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    17863 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16912 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.595877 dm-haiku-0.0.9/dm_haiku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17863 2022-11-16 12:15:30.000000 dm-haiku-0.0.9/dm_haiku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4293 2022-11-16 12:15:30.000000 dm-haiku-0.0.9/dm_haiku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 12:15:30.000000 dm-haiku-0.0.9/dm_haiku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 12:15:30.000000 dm-haiku-0.0.9/dm_haiku.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2022-11-16 12:15:30.000000 dm-haiku-0.0.9/dm_haiku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2022-11-16 12:15:30.000000 dm-haiku-0.0.9/dm_haiku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.595877 dm-haiku-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7617 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.595877 dm-haiku-0.0.9/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/docs/ext/coverage_check.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.587877 dm-haiku-0.0.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.595877 dm-haiku-0.0.9/examples/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/imagenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11100 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/imagenet/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13269 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/imagenet/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.599877 dm-haiku-0.0.9/examples/impala/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5627 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/actor_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4319 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/agent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5316 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/haiku_nets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7684 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/learner_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/run_catch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/impala/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.599877 dm-haiku-0.0.9/examples/rnn/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/rnn/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6605 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/rnn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.599877 dm-haiku-0.0.9/examples/transformer/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/transformer/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/transformer/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5406 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/examples/transformer/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.603877 dm-haiku-0.0.9/haiku/
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.623878 dm-haiku-0.0.9/haiku/_src/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6402 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4888 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40107 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28859 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12002 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8184 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8580 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8676 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/batch_norm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6022 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/bias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/bias_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10482 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4695 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32135 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28811 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10819 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14051 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/data_structures_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5121 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/deferred_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13407 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12738 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/depthwise_conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13253 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/dot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4412 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/dot_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7997 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3751 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/embed_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/eval_shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2981 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/eval_shape_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13860 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/filtering_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8887 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/group_norm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10706 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/group_norm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11827 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7869 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/initializers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/haiku/_src/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/check_tracer_leaks_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/checkpoint_generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2089 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2100 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12749 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/descriptors_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4074 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/doctest_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/float64_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/half_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/hk_transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2798 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/jax2tf_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/jax_transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/jaxpr_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3436 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/numpy_inputs_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/rank_promotion_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/replaceable_funcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/shim_hk_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/summarise_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/to_dot_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/integration/typing_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22664 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/jaxpr_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4768 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/jaxpr_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9998 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9359 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/layer_norm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9926 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17843 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/layer_stack_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18779 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/lift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19086 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/lift_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8577 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7313 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/mixed_precision_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28752 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32641 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/module_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7772 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/moving_averages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9498 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/moving_averages_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11720 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/multi_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4595 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/multi_transform_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/haiku/_src/nets/
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5834 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/mlp_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5088 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/mobilenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/mobilenetv1_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21716 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6714 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14856 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/vqvae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8055 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/nets/vqvae_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4442 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/pad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2835 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/pad_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7420 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9267 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/pool_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/random.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28064 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19197 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5567 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4592 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/reshape_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/rms_norm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5090 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/rms_norm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6752 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/spectral_norm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/spectral_norm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34322 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32550 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/stateful_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15463 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/summarise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8856 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/summarise_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7848 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/test_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21738 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2307 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/typing_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9176 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5781 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/_src/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/haiku/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/benchmarks/eval_shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/benchmarks/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/data_structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/haiku/experimental/
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/experimental/jaxpr_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/nets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/pad.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/haiku/typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/requirements-jax.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-16 12:15:30.627878 dm-haiku-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2679 2022-11-16 12:15:17.000000 dm-haiku-0.0.9/setup.py
```

### Comparing `dm-haiku-0.0.8/LICENSE` & `dm-haiku-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/PKG-INFO` & `dm-haiku-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-haiku
-Version: 0.0.8
+Version: 0.0.9
 Summary: Haiku is a library for building neural networks in JAX.
 Home-page: https://github.com/deepmind/dm-haiku
 Author: DeepMind
 Author-email: haiku-dev-os@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -448,15 +448,15 @@
 To cite this repository:
 
 ```
 @software{haiku2020github,
   author = {Tom Hennigan and Trevor Cai and Tamara Norman and Igor Babuschkin},
   title = {{H}aiku: {S}onnet for {JAX}},
   url = {http://github.com/deepmind/dm-haiku},
-  version = {0.0.3},
+  version = {0.0.9},
   year = {2020},
 }
 ```
 
 In this bibtex entry, the version number is intended to be from
 [`haiku/__init__.py`](https://github.com/deepmind/dm-haiku/blob/main/haiku/__init__.py),
 and the year corresponds to the project's open-source release.
```

### Comparing `dm-haiku-0.0.8/README.md` & `dm-haiku-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 To cite this repository:
 
 ```
 @software{haiku2020github,
   author = {Tom Hennigan and Trevor Cai and Tamara Norman and Igor Babuschkin},
   title = {{H}aiku: {S}onnet for {JAX}},
   url = {http://github.com/deepmind/dm-haiku},
-  version = {0.0.3},
+  version = {0.0.9},
   year = {2020},
 }
 ```
 
 In this bibtex entry, the version number is intended to be from
 [`haiku/__init__.py`](https://github.com/deepmind/dm-haiku/blob/main/haiku/__init__.py),
 and the year corresponds to the project's open-source release.
```

### Comparing `dm-haiku-0.0.8/dm_haiku.egg-info/PKG-INFO` & `dm-haiku-0.0.9/dm_haiku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-haiku
-Version: 0.0.8
+Version: 0.0.9
 Summary: Haiku is a library for building neural networks in JAX.
 Home-page: https://github.com/deepmind/dm-haiku
 Author: DeepMind
 Author-email: haiku-dev-os@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -448,15 +448,15 @@
 To cite this repository:
 
 ```
 @software{haiku2020github,
   author = {Tom Hennigan and Trevor Cai and Tamara Norman and Igor Babuschkin},
   title = {{H}aiku: {S}onnet for {JAX}},
   url = {http://github.com/deepmind/dm-haiku},
-  version = {0.0.3},
+  version = {0.0.9},
   year = {2020},
 }
 ```
 
 In this bibtex entry, the version number is intended to be from
 [`haiku/__init__.py`](https://github.com/deepmind/dm-haiku/blob/main/haiku/__init__.py),
 and the year corresponds to the project's open-source release.
```

### Comparing `dm-haiku-0.0.8/dm_haiku.egg-info/SOURCES.txt` & `dm-haiku-0.0.9/dm_haiku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/docs/conf.py` & `dm-haiku-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/docs/ext/coverage_check.py` & `dm-haiku-0.0.9/docs/ext/coverage_check.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/imagenet/__init__.py` & `dm-haiku-0.0.9/examples/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/imagenet/dataset.py` & `dm-haiku-0.0.9/examples/imagenet/dataset.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/imagenet/train.py` & `dm-haiku-0.0.9/examples/imagenet/train.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/__init__.py` & `dm-haiku-0.0.9/examples/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/actor.py` & `dm-haiku-0.0.9/examples/impala/actor.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/actor_test.py` & `dm-haiku-0.0.9/examples/impala/actor_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/agent.py` & `dm-haiku-0.0.9/examples/impala/agent.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/haiku_nets.py` & `dm-haiku-0.0.9/examples/impala/haiku_nets.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/learner.py` & `dm-haiku-0.0.9/examples/impala/learner.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/learner_test.py` & `dm-haiku-0.0.9/examples/impala/learner_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/run_catch.py` & `dm-haiku-0.0.9/examples/impala/run_catch.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/impala/util.py` & `dm-haiku-0.0.9/examples/impala/util.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/rnn/__init__.py` & `dm-haiku-0.0.9/examples/rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/rnn/dataset.py` & `dm-haiku-0.0.9/examples/rnn/dataset.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/rnn/train.py` & `dm-haiku-0.0.9/examples/rnn/train.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/transformer/__init__.py` & `dm-haiku-0.0.9/examples/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/transformer/dataset.py` & `dm-haiku-0.0.9/examples/transformer/dataset.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/transformer/model.py` & `dm-haiku-0.0.9/examples/transformer/model.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/examples/transformer/train.py` & `dm-haiku-0.0.9/examples/transformer/train.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/__init__.py` & `dm-haiku-0.0.9/haiku/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 from haiku._src.transform import without_state
 from haiku._src.typing import ModuleProtocol
 from haiku._src.typing import Params
 from haiku._src.typing import State
 from haiku._src.typing import SupportsCall
 from haiku._src.utils import get_channel_index
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 __all__ = (
     "AvgPool",
     "BatchApply",
     "BatchNorm",
     "Bias",
     "Conv1D",
```

### Comparing `dm-haiku-0.0.8/haiku/_src/__init__.py` & `dm-haiku-0.0.9/haiku/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/analytics.py` & `dm-haiku-0.0.9/haiku/_src/analytics.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/attention.py` & `dm-haiku-0.0.9/haiku/_src/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,17 @@
   ):
     """Initialises the module.
 
     Args:
       num_heads: Number of independent attention heads (H).
       key_size: The size of keys (K) and queries used for attention.
       w_init_scale: DEPRECATED. Please use w_init instead.
-      w_init: Initialiser for weights in the linear map.
+      w_init: Initialiser for weights in the linear map. Once `w_init_scale` is
+        fully deprecated `w_init` will become mandatory. Until then it has a
+        default value of `None` for backwards compatability.
       value_size: Optional size of the value projection (V). If None, defaults
         to the key size (K).
       model_size: Optional size of the output embedding (D'). If None, defaults
         to the key size multiplied by the number of heads (K * H).
       name: Optional name for this module.
     """
     super().__init__(name=name)
@@ -88,15 +90,17 @@
     if w_init_scale is not None:
       warnings.warn(
           "w_init_scale is deprecated; please pass an explicit weight "
           "initialiser instead.", DeprecationWarning)
     if w_init and w_init_scale:
       raise ValueError("Please provide only `w_init`, not `w_init_scale`.")
     if w_init is None and w_init_scale is None:
-      raise ValueError("Please provide a weight initializer: `w_init`.")
+      raise ValueError("Please provide a weight initializer: `w_init`. "
+                       "`w_init` will become mandatory once `w_init_scale` is "
+                       "fully deprecated.")
     if w_init is None:
       w_init = hk.initializers.VarianceScaling(w_init_scale)
     self.w_init = w_init
 
   def __call__(
       self,
       query: jnp.ndarray,
```

### Comparing `dm-haiku-0.0.8/haiku/_src/attention_test.py` & `dm-haiku-0.0.9/haiku/_src/attention_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/base.py` & `dm-haiku-0.0.9/haiku/_src/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,16 +466,16 @@
     name: str,
     shape: Sequence[int],
     dtype: Any = jnp.float32,
     init: Optional[Initializer] = None,
 ) -> jnp.ndarray:
   """Creates or reuses a parameter for the given transformed function.
 
-  >>> hk.get_parameter("w", [], init=jnp.ones)
-  DeviceArray(1., dtype=float32)
+  >>> print(hk.get_parameter("w", [], init=jnp.ones))
+  1.0
 
   Parameters within the same :func:`transform` and/or :class:`Module` with the
   same name have the same value:
 
   >>> w1 = hk.get_parameter("w", [], init=jnp.zeros)
   >>> w2 = hk.get_parameter("w", [], init=jnp.zeros)
   >>> assert w1 is w2
@@ -617,24 +617,24 @@
 
   >>> def zeros_creator(next_creator, shape, dtype, init, context):
   ...   init = jnp.zeros
   ...   return next_creator(shape, dtype, init)
 
   >>> with hk.custom_creator(zeros_creator):
   ...   z = hk.get_parameter("z", [], jnp.float32, jnp.ones)
-  >>> z
-  DeviceArray(0., dtype=float32)
+  >>> print(z)
+  0.0
 
   If ``state=True`` then your creator will additionally run on calls to
   :func:`get_state`:
 
   >>> with hk.custom_creator(zeros_creator, state=True):
   ...   z = hk.get_state("z", [], jnp.float32, jnp.ones)
-  >>> z
-  DeviceArray(0., dtype=float32)
+  >>> print(z)
+  0.0
 
   Args:
     creator: A parameter creator.
     params: Whether to intercept parameter creation, defaults to ``True``.
     state: Whether to intercept state creation, defaults to ``False``.
 
   Returns:
@@ -775,27 +775,27 @@
     _, name = self.full_name.rsplit("/", 1)
     return name
 
 
 def custom_setter(setter: Setter) -> contextlib.AbstractContextManager:
   """Registers a custom state setter.
 
-  When state is set using :func:`get_parameter` we always run all custom setters
+  When state is set using :func:`set_state` we always run all custom setters
   before saving the value.
 
   >>> def zero_during_init(next_setter, value, context):
   ...   if hk.running_init():
   ...     value = jnp.zeros_like(value)
   ...   return next_setter(value)
 
   >>> with hk.custom_setter(zero_during_init):
   ...   hk.set_state("x", jnp.ones([2]))
   ...   x = hk.get_state("x")
-  >>> x
-  DeviceArray([0., 0.], dtype=float32)
+  >>> print(x)
+  [0. 0.]
 
   Args:
     setter: A state setter.
 
   Returns:
     Context manager under which the setter is active.
   """
@@ -881,20 +881,20 @@
       #
       # Where subkey1->subkey4 are provided to the user in order when requested.
       new_keys = tuple(jax.random.split(self._key, num + 1))
       self._key = new_keys[0]
       self._subkeys.extend(new_keys[1:])
 
   def reserve_up_to_full(self):
-    reserve_size = config.get_config().rng_reserve_size
-    num = reserve_size - len(self._subkeys)
-    if num > 0:
-      self.reserve(num)
-    else:
-      sliced_subkeys = list(self._subkeys)[:reserve_size]
+    num = config.get_config().rng_reserve_size
+    diffnum = num - len(self._subkeys)
+    if diffnum > 0:
+      self.reserve(diffnum)
+    elif diffnum < 0:
+      sliced_subkeys = list(self._subkeys)[:num]
       self._subkeys = collections.deque(sliced_subkeys)
 
   @property
   def internal_state(self) -> PRNGSequenceState:
     return self._key, tuple(self._subkeys)
 
   def replace_internal_state(self, state: PRNGSequenceState):
@@ -1056,22 +1056,22 @@
 
   "State" can be used to represent mutable state in your network. The most
   common usage of state is to represent the moving averages used in batch
   normalization (see :class:`ExponentialMovingAverage`). If your network uses
   "state" then you are required to use :func:`transform_with_state` and pass
   state into and out of the apply function.
 
-  >>> hk.get_state("counter", [], init=jnp.zeros)
-  DeviceArray(0., dtype=float32)
+  >>> print(hk.get_state("counter", [], init=jnp.zeros))
+  0.0
 
   If the value for the given state is already defined (e.g. using
   :func:`set_state`) then you can call with just the name:
 
-  >>> hk.get_state("counter")
-  DeviceArray(0., dtype=float32)
+  >>> print(hk.get_state("counter"))
+  0.0
 
   MOTE: state within the same :func:`transform` and/or :class:`Module` with the
   same name have the same value:
 
   >>> c1 = hk.get_state("counter")
   >>> c2 = hk.get_state("counter")
   >>> assert c1 is c2
@@ -1132,16 +1132,16 @@
   "State" can be used to represent mutable state in your network. The most
   common usage of state is to represent the moving averages used in batch
   normalization (see :class:`ExponentialMovingAverage`). If your network uses
   "state" then you are required to use :func:`transform_with_state` and pass
   state into and out of the apply function.
 
   >>> hk.set_state("counter", jnp.zeros([]))
-  >>> hk.get_state("counter")
-  DeviceArray(0., dtype=float32)
+  >>> print(hk.get_state("counter"))
+  0.0
 
   NOTE: state within the same :func:`transform` and/or :class:`Module` with the
   same name have the same value:
 
   >>> w1 = hk.get_state("counter")
   >>> w2 = hk.get_state("counter")
   >>> assert w1 is w2
@@ -1256,15 +1256,17 @@
   """Asserts that in the given block params, state and rng are unchanged."""
   params_before, state_before, rng_before = _all_state()
   yield
   params_after, state_after, rng_after = _all_state()
 
   params_diff = params_after - params_before
   state_diff = state_after - state_before
-  rng_diff = rng_after - rng_before
+  # Amount of rng keys can increase (reserve_rng_keys) or decrease
+  # (next_rng_key), so need symmetric set difference (^).
+  rng_diff = rng_after ^ rng_before
   if params_diff or state_diff or rng_diff:
     raise StateChangedError("Within this code block you are not able to modify "
                             "Haiku managed state (e.g. via `next_rng_key` or "
                             "`set_state`).")
 
 
 class StateChangedError(AssertionError):
```

### Comparing `dm-haiku-0.0.8/haiku/_src/base_test.py` & `dm-haiku-0.0.9/haiku/_src/base_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/basic.py` & `dm-haiku-0.0.9/haiku/_src/basic.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/basic_test.py` & `dm-haiku-0.0.9/haiku/_src/basic_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/batch_norm.py` & `dm-haiku-0.0.9/haiku/_src/batch_norm.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/batch_norm_test.py` & `dm-haiku-0.0.9/haiku/_src/batch_norm_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/bias.py` & `dm-haiku-0.0.9/haiku/_src/bias.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/bias_test.py` & `dm-haiku-0.0.9/haiku/_src/bias_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/config.py` & `dm-haiku-0.0.9/haiku/_src/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,16 @@
   >>> jax.vmap(f, axis_size=2)()
   Traceback (most recent call last):
     ...
   haiku.JaxUsageError: ...
 
   Using the Haiku wrapped version works correctly:
 
-  >>> hk.vmap(f, axis_size=2, split_rng=False)()
-  DeviceArray([0., 0.], dtype=float32)
+  >>> print(hk.vmap(f, axis_size=2, split_rng=False)())
+  [0. 0.]
 
   Args:
     enabled: Boolean indicating whether usage should be checked or not.
 
   Returns:
     Boolean with the previous value for this setting.
   """
```

### Comparing `dm-haiku-0.0.8/haiku/_src/config_test.py` & `dm-haiku-0.0.9/haiku/_src/config_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/conv.py` & `dm-haiku-0.0.9/haiku/_src/conv.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/conv_test.py` & `dm-haiku-0.0.9/haiku/_src/conv_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/data_structures.py` & `dm-haiku-0.0.9/haiku/_src/data_structures.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/data_structures_test.py` & `dm-haiku-0.0.9/haiku/_src/data_structures_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/deferred.py` & `dm-haiku-0.0.9/haiku/_src/deferred.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/deferred_test.py` & `dm-haiku-0.0.9/haiku/_src/deferred_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/depthwise_conv.py` & `dm-haiku-0.0.9/haiku/_src/depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/depthwise_conv_test.py` & `dm-haiku-0.0.9/haiku/_src/depthwise_conv_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/dot.py` & `dm-haiku-0.0.9/haiku/_src/dot.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/dot_test.py` & `dm-haiku-0.0.9/haiku/_src/dot_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/embed.py` & `dm-haiku-0.0.9/haiku/_src/embed.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/embed_test.py` & `dm-haiku-0.0.9/haiku/_src/embed_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/eval_shape.py` & `dm-haiku-0.0.9/haiku/_src/eval_shape.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/eval_shape_test.py` & `dm-haiku-0.0.9/haiku/_src/eval_shape_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/filtering.py` & `dm-haiku-0.0.9/haiku/_src/filtering.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/filtering_test.py` & `dm-haiku-0.0.9/haiku/_src/filtering_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/group_norm.py` & `dm-haiku-0.0.9/haiku/_src/group_norm.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/group_norm_test.py` & `dm-haiku-0.0.9/haiku/_src/group_norm_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/initializers.py` & `dm-haiku-0.0.9/haiku/_src/initializers.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/initializers_test.py` & `dm-haiku-0.0.9/haiku/_src/initializers_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/__init__.py` & `dm-haiku-0.0.9/haiku/_src/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/check_tracer_leaks_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/check_tracer_leaks_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/checkpoint_generate.py` & `dm-haiku-0.0.9/haiku/_src/integration/checkpoint_generate.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/checkpoint_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/checkpoint_utils.py` & `dm-haiku-0.0.9/haiku/_src/integration/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/common.py` & `dm-haiku-0.0.9/haiku/_src/integration/common.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/descriptors.py` & `dm-haiku-0.0.9/haiku/_src/integration/descriptors.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/descriptors_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/descriptors_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/doctest_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/doctest_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/float64_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/float64_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/half_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/half_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/hk_transforms_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/hk_transforms_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/jax2tf_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/jax2tf_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/jax_transforms_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/jax_transforms_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/jaxpr_info_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/jaxpr_info_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/numpy_inputs_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/numpy_inputs_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests whether modules produce similar output given np.ndarray inputs."""
 
 import functools
-from typing import Tuple
+import os
+from typing import Tuple, Type
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import haiku as hk
 from haiku._src import test_utils
 from haiku._src.integration import descriptors
 import jax
@@ -30,14 +31,19 @@
 
 
 def tree_assert_allclose(a, b, *, atol=1e-6):
   jax.tree_util.tree_map(
       functools.partial(np.testing.assert_allclose, atol=atol), a, b)
 
 
+def get_module_cls(module_fn: ModuleFn) -> Type[hk.Module]:
+  get_cls = lambda: type(descriptors.unwrap(module_fn()))
+  return hk.testing.transform_and_run(get_cls)()
+
+
 class NumpyInputsTest(parameterized.TestCase):
 
   @test_utils.combined_named_parameters(
       descriptors.ALL_MODULES,
       test_utils.named_bools('np_inputs'),
       test_utils.named_bools('np_params'),
       test_utils.named_bools('close_over_params'))
@@ -49,14 +55,21 @@
       np_params: bool,
       np_inputs: bool,
       close_over_params: bool,
   ):
     if not (np_params or np_inputs):
       self.skipTest('Pure JAX variants tested elsewhere')
 
+    # TODO(b/257921991): Fix the timeouts here.
+    if (close_over_params and 'UNITTEST_ON_FORGE' in os.environ):
+      module_cls = get_module_cls(module_fn)
+      if module_cls in (hk.nets.ResNet, hk.Conv2DTranspose, hk.LayerNorm,
+                        hk.Conv2DLSTM, hk.IdentityCore):
+        self.skipTest('Close over tests for these modules take >5 minutes')
+
     f = hk.transform_with_state(lambda x: module_fn()(x))  # pylint: disable=unnecessary-lambda
 
     rng = jax.random.PRNGKey(42)
     x = jnp.ones(shape, dtype)
     params, state = f.init(rng, x)
     if close_over_params:
       apply_fn = functools.partial(f.apply, params, state)
```

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/rank_promotion_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/rank_promotion_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/replaceable_funcs_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/replaceable_funcs_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/shim_hk_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/shim_hk_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/summarise_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/summarise_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/to_dot_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/to_dot_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/integration/typing_test.py` & `dm-haiku-0.0.9/haiku/_src/integration/typing_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/jaxpr_info.py` & `dm-haiku-0.0.9/haiku/_src/jaxpr_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 
 Example usage:
 
     mod = jaxpr_info.make_model_info(my_callable)(some, arguments)
     print(jaxpr_info.format_module(mod))
 
 """
+import contextlib
 import dataclasses
 import itertools
 import logging
 import os
 import sys
-from typing import Any, Callable, Dict, List, Mapping, NamedTuple, Set, Sequence, Optional
+from typing import Any, Callable, Dict, List, Mapping, NamedTuple, Set, Sequence, Optional, Tuple
 
 from haiku._src import summarise
 import jax
+from jax.experimental import maps
 
 
 @dataclasses.dataclass
 class Module:
   """Information about a Haiku module."""
   # Name of the module, e.g. the Haiku module name.
   name: str
@@ -98,72 +100,96 @@
   # For internal use, the name scope stack of this expression.
   name_stack: Sequence[str] = dataclasses.field(default_factory=list)
 
 
 ComputeFlopsFn = Callable[[jax.core.JaxprEqn, Expression], int]
 
 
+# TODO(yashkatariya): Remove once jax.Array is ready
+@contextlib.contextmanager
+def _maybe_set_global_semantics():
+  """Sets global semantics within the context manager.
+
+  Required for evaluating make_jaxpr on GlobalDeviceArray values.
+
+  Yields:
+    No value, but a JAX environment which sets GLOBAL positional semantics.
+  """
+  prev_positional_val = maps._positional_semantics.val  # pylint: disable=protected-access
+  try:
+    if jax.config.jax_parallel_functions_output_gda:
+      maps._positional_semantics.val = maps._PositionalSemantics.GLOBAL  # pylint: disable=protected-access
+    yield
+  finally:
+    maps._positional_semantics.val = prev_positional_val  # pylint: disable=protected-access
+
+
 def make_model_info(
     f: Callable[..., Any],
     name: Optional[str] = None,
     include_module_info: bool = True,
     compute_flops: Optional[ComputeFlopsFn] = None,
+    axis_env: Optional[Sequence[Tuple[Any, int]]] = None,
 ) -> Callable[..., Module]:
   """Creates a function that computes flop, param and state information.
 
   Requires hk.experimental.profiler_name_scopes(enabled=True).
 
   Args:
     f: The function for which to compute information. Haiku modules and
       jax.named_call expressions will be represented as nested Modules in the
       result.
     name: Optional, the name of the root expression.
     include_module_info: Whether to include parameter and state count
       information for haiku modules. Can be slow for very large computations.
     compute_flops: Optional, a function that returns an estimate of the number
       of flops required to execute an equation.
+    axis_env: Sizes of pmapped axes.  See docs of jax.make_jaxpr for details.
 
   Returns:
     A wrapped version of `f` that when applied to example arguments returns a
     `Module` representation of `f` for those arguments.
 
   `Module` and `Expression` contain high level information about JAX operations
   (jaxprs) and can be visualized in concise and interactive formats; see
   `format_module`, `as_html_page` or `as_html`.
   """
   if not name:
     name = f.__name__
-  make_jaxpr = jax.make_jaxpr(f)
+  make_jaxpr = jax.make_jaxpr(f, axis_env=axis_env)
   if include_module_info:
     # Wrap f in a lambda so eval_summary doesn't try to un-transform it.
     # TODO(tomhennigan): remove lambda trick
     make_module_info = summarise.eval_summary(lambda *a, **k: f(*a, **k))  # pylint: disable=unnecessary-lambda
 
   def make_module(*args, **kwargs):
     old_limit = sys.getrecursionlimit()
 
     try:
       # Increase recursion limit as graphs may be very deep
       sys.setrecursionlimit(int(10e3))
 
+      with _maybe_set_global_semantics():
+        jaxpr = make_jaxpr(*args, **kwargs).jaxpr
+
       # Compute flops for all expressions.
       module = Module(name=name)
       _process_jaxpr(
-          make_jaxpr(*args, **kwargs).jaxpr,
+          jaxpr,
           compute_flops,
           scope=_ModuleScope(named_call_id='0'),
           seen=set(),
           module=module)
 
-      if jax.config.jax_experimental_name_stack:
-        _name_scopes_to_modules(module)
+      _name_scopes_to_modules(module)
 
       if include_module_info:
         # Add haiku param and state counts for all haiku modules.
-        module_infos = make_module_info(*args, **kwargs)
+        with _maybe_set_global_semantics():
+          module_infos = make_module_info(*args, **kwargs)
         by_name = {i.module_details.module.module_name: i for i in module_infos}
         by_name = {k.replace('/~/', '/'): v for k, v in by_name.items()}
 
         for expr in module.expressions:
           if expr.submodule:
             _add_param_counts(expr.submodule, expr.submodule.name, by_name)
     finally:
```

### Comparing `dm-haiku-0.0.8/haiku/_src/jaxpr_info_test.py` & `dm-haiku-0.0.9/haiku/_src/jaxpr_info_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,22 +37,18 @@
 
 
 class JaxprInfoTest(absltest.TestCase):
 
   def setUp(self):
     super().setUp()
     self.prev_profiler_name_scopes = config.profiler_name_scopes(enabled=True)
-    self.prev_experimental_namestack = jax.config.jax_experimental_name_stack
-    jax.config.update("jax_experimental_name_stack", True)
 
   def tearDown(self):
     super().tearDown()
     config.profiler_name_scopes(self.prev_profiler_name_scopes)
-    jax.config.update("jax_experimental_name_stack",
-                      self.prev_experimental_namestack)
 
   def test_simple_expression(self):
 
     def add(x, y):
       return jnp.sign(x) + jnp.cos(y)
 
     a = jnp.zeros((12, 7))
```

### Comparing `dm-haiku-0.0.8/haiku/_src/layer_norm.py` & `dm-haiku-0.0.9/haiku/_src/layer_norm.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/layer_norm_test.py` & `dm-haiku-0.0.9/haiku/_src/layer_norm_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/layer_stack.py` & `dm-haiku-0.0.9/haiku/_src/layer_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,17 +245,16 @@
   >>> num_layers = 4
   >>> x = 0
   >>> ys_0 = jnp.array([1, 2, 3, 4])
   >>> ys_1 = jnp.array([5, 6, 7, 8])
   >>> stack = hk.experimental.layer_stack(num_layers,
   ...                                     with_per_layer_inputs=True)
   >>> x, zs = stack(f)(x, ys_0, ys_1)
-  >>> x, zs
-  (DeviceArray(4, dtype=int32, weak_type=True),
-      DeviceArray([ 6,  8, 10, 12], dtype=int32))
+  >>> print(x, zs)
+  4 [ 6  8 10 12]
 
   Check the tests in ``layer_stack_test.py`` for further examples.
 
   Crucially, any parameters created inside ``f`` will not be shared across
   iterations.
 
   Args:
```

### Comparing `dm-haiku-0.0.8/haiku/_src/layer_stack_test.py` & `dm-haiku-0.0.9/haiku/_src/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/lift.py` & `dm-haiku-0.0.9/haiku/_src/lift.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,14 +130,20 @@
     init_fn: Callable[..., hk.Params],
     *,
     allow_reuse: bool = False,
     name: str = "lifted",
 ) -> Callable[..., hk.Params]:
   r"""Registers parameters from an inner init function in an outer transform.
 
+  HINT: :func:`lift` is for when you want to make non-trivial use of JAX
+  transforms (e.g. ``jax.vmap``) **inside** of a :func:`transform` or
+  :func:`transform_with_state`. We generally recommend trying to use JAX
+  transforms on the pure functions returned by :func:`transform`, in which case
+  you do not need :func:`lift`.
+
   Use :func:`lift`\ when nesting Haiku transforms to register the parameters of
   the inner transform in any outer transform. This is mainly useful when using
   JAX functions inside of a Haiku module (eg. using ``jax.vmap`` on a layer).
   See
   https://dm-haiku.readthedocs.io/en/latest/notebooks/transforms.html#Using-hk.lift
   for more explanation of when to use :func:`lift`\ . (If you're not using JAX
   functions inside of a module or don't need access to your parameters inside of
@@ -153,24 +159,72 @@
 
   By default, users must ensure that the given ``init`` does not accidentally
   catch modules from an outer :func:`transform` via functional
   closure. If this behavior is desirable, set ``allow_reuse`` to ``True``.
 
   Example:
 
-    >>> # outer can be `hk.transform`ed and will contain the params of inner.
-    >>> def outer(x):
-    ...   @hk.transform
-    ...   def inner(x):
-    ...     return hk.Linear(1)(x)
-    ...   init_rng = hk.next_rng_key() if hk.running_init() else None
-    ...   x = jnp.ones([1, 1])
-    ...   params = hk.lift(inner.init, name='f_lift')(init_rng, x)
-    ...   # inner.apply is a pure function and can be vmapped.
-    ...   return jax.vmap(inner.apply, in_axes=(0, None, 0))(params, None, x)
+  A common usage of :func:`lift` is to use JAX transformations like ``vmap`` in
+  non-trivial ways, inside a :func:`transform`. For example, we can use
+  :func:`lift` and ``jax.vmap`` to create an ensemble.
+
+  First we'll create a helper function that uses :func:`lift` to apply ``vmap``
+  to our model. As you can see from the comments, we are using ``vmap`` to
+  change how parameters should be created (in this case we create a unique set
+  of parameters for each member of the ensemble) and we change how apply works
+  (we "map" the parameters meaning JAX will compute the forward pass separately,
+  in parallel, for each member of the ensemble):
+
+  >>> def create_ensemble(model, size: int):
+  ...   init_rng = hk.next_rng_keys(size) if hk.running_init() else None
+  ...   model = hk.transform(model)
+  ...   # in_axes: rng is mapped, data is not.
+  ...   init_model = jax.vmap(model.init, in_axes=(0, None))
+  ...   # Use hk.lift to "lift" parameters created by `init_model` into the
+  ...   # outer transform.
+  ...   init_model = hk.lift(init_model, name="ensemble")
+  ...   def ensemble(x):
+  ...     params = init_model(init_rng, x)
+  ...     # in_axes: params are mapped, rng/data are not.
+  ...     return jax.vmap(model.apply, in_axes=(0, None, None))(params, None, x)
+  ...   return ensemble
+
+  We can now use this function to ensemble any Haiku module(s), inside of a
+  transform. First we define a function for each member of the ensemble:
+
+  >>> def member_fn(x):
+  ...   return hk.nets.MLP([300, 100, 10])(x)
+
+  Secondly we can combine our two functions, inside a :func:`transform` to
+  create an ensemble:
+
+  >>> def f(x):
+  ...   ensemble = create_ensemble(member_fn, size=4)
+  ...   x = ensemble(x)
+  ...   # You could create other modules here which were not ensembled.
+  ...   return x
+  >>> f = hk.transform(f)
+
+  When we initialize the network, our ensemble member's parameters have a
+  leading dimension the size of the ensemble:
+
+  >>> rng = jax.random.PRNGKey(777)
+  >>> x = jnp.ones([32, 128])
+  >>> params = f.init(rng, x)
+  >>> jax.tree_util.tree_map(lambda x: x.shape, params)
+  {'ensemble/mlp/~/linear_0': {'b': (4, 300), 'w': (4, 128, 300)},
+   'ensemble/mlp/~/linear_1': {'b': (4, 100), 'w': (4, 300, 100)},
+   'ensemble/mlp/~/linear_2': {'b': (4, 10), 'w': (4, 100, 10)}}
+
+  When we apply the network, we get an output for each member of the ensemble
+  for the entire batch:
+
+  >>> y = f.apply(params, None, x)
+  >>> y.shape
+  (4, 32, 10)
 
   Args:
     init_fn: The ``init`` function from an :class:`Transformed`\ .
     allow_reuse: Allows lifted parameters and state to be reused from the
       outer :func:`transform`. This can be desirable when using ``lift`` within
       control flow (e.g. ``hk.scan``).
     name: A string name to prefix parameters with.
```

### Comparing `dm-haiku-0.0.8/haiku/_src/lift_test.py` & `dm-haiku-0.0.9/haiku/_src/lift_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/mixed_precision.py` & `dm-haiku-0.0.9/haiku/_src/mixed_precision.py`

 * *Files 10% similar despite different names*

```diff
@@ -152,32 +152,32 @@
   parameters in ``float32``, but cast them to ``float16`` before use, along with
   all module inputs:
 
   >>> policy = jmp.get_policy('params=float32,compute=float16,output=float32')
   >>> hk.mixed_precision.set_policy(hk.nets.ResNet50, policy)
   >>> net = hk.nets.ResNet50(4)
   >>> x = jnp.ones([4, 224, 224, 3])
-  >>> net(x, is_training=True)
-  DeviceArray([[nan, nan, nan, nan],
-               [nan, nan, nan, nan],
-               [nan, nan, nan, nan],
-               [nan, nan, nan, nan]], dtype=float32)
+  >>> print(net(x, is_training=True))
+  [[nan nan nan nan]
+   [nan nan nan nan]
+   [nan nan nan nan]
+   [nan nan nan nan]]
 
   Oh no, nan! This is because modules like batch norm are not numerically stable
   in ``float16``. To address this, we apply a second policy to our batch norm
   modules to keep them in full precision. We are careful to return a ``float16``
   output from the module such that subsequent modules receive ``float16`` input:
 
   >>> policy = jmp.get_policy('params=float32,compute=float32,output=float16')
   >>> hk.mixed_precision.set_policy(hk.BatchNorm, policy)
-  >>> net(x, is_training=True)
-  DeviceArray([[0., 0., 0., 0.],
-               [0., 0., 0., 0.],
-               [0., 0., 0., 0.],
-               [0., 0., 0., 0.]], dtype=float32)
+  >>> print(net(x, is_training=True))
+  [[0. 0. 0. 0.]
+   [0. 0. 0. 0.]
+   [0. 0. 0. 0.]
+   [0. 0. 0. 0.]]
 
   For a fully worked mixed precision example see the imagenet example in Haiku's
   examples directory. This example shows mixed precision on GPU offering a 2x
   speedup in training time with only a small impact on final top-1 accuracy.
 
   >>> hk.mixed_precision.clear_policy(hk.nets.ResNet50)
   >>> hk.mixed_precision.clear_policy(hk.BatchNorm)
```

### Comparing `dm-haiku-0.0.8/haiku/_src/mixed_precision_test.py` & `dm-haiku-0.0.9/haiku/_src/mixed_precision_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/module.py` & `dm-haiku-0.0.9/haiku/_src/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import sys
 from typing import (Any, Callable, ContextManager, Dict, Mapping, NamedTuple,
                     Optional, Set, Tuple, Type, TypeVar)
 
 from haiku._src import base
 from haiku._src import config
 from haiku._src import data_structures
-from haiku._src import stateful
 from haiku._src import utils
 import jax
 import jax.numpy as jnp
 
 # pylint: disable=g-import-not-at-top
 if sys.version_info < (3, 8):
   from typing_extensions import Protocol
@@ -414,26 +413,19 @@
     frame = base.current_frame()
     state = base.ModuleState(module=self, method_name=submodule_method_name)
     with frame.module(state), _module_method_call(self, method_name):
       # hk.Module enters the module name scope for all methods.
       module_name = getattr(self, "module_name", None)
       f = functools.partial(unbound_method, self)
       f = functools.partial(run_interceptors, f, method_name, self)
-      if jax.config.jax_experimental_name_stack and module_name:
+      if module_name:
         local_module_name = module_name.split("/")[-1]
         f = jax.named_call(f, name=local_module_name)
         if method_name != "__call__":
           f = jax.named_call(f, name=method_name)
-      elif module_name:
-        # TODO(lenamartens): remove this branch once jax_experimental_name_stack
-        # flag is removed.
-        cfg = config.get_config()
-        if cfg.profiler_name_scopes and method_name == "__call__":
-          local_module_name = module_name.split("/")[-1]
-          f = stateful.named_call(f, name=local_module_name)
 
       out = f(*args, **kwargs)
 
       # Module names are set in the constructor. If `f` is the constructor then
       # its name will only be set **after** `f` has run. For methods other
       # than `__init__` we need the name before running in order to wrap their
       # execution with `named_call`.
@@ -594,16 +586,16 @@
   ...   mod = AddModule()
   ...   return mod(x)
 
   >>> forward = hk.transform(forward_fn)
   >>> x = 1.
   >>> rng = None
   >>> params = forward.init(rng, x)
-  >>> forward.apply(params, None, x)
-  DeviceArray(2., dtype=float32)
+  >>> print(forward.apply(params, None, x))
+  2.0
   """
 
   def __init__(self, name: Optional[str] = None):
     """Initializes the current module with the given name.
 
     Subclasses should call this constructor before creating other modules or
     variables such that those modules are named correctly.
```

### Comparing `dm-haiku-0.0.8/haiku/_src/module_test.py` & `dm-haiku-0.0.9/haiku/_src/module_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/moving_averages.py` & `dm-haiku-0.0.9/haiku/_src/moving_averages.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/moving_averages_test.py` & `dm-haiku-0.0.9/haiku/_src/moving_averages_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/multi_transform.py` & `dm-haiku-0.0.9/haiku/_src/multi_transform.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/multi_transform_test.py` & `dm-haiku-0.0.9/haiku/_src/multi_transform_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/__init__.py` & `dm-haiku-0.0.9/haiku/_src/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/mlp.py` & `dm-haiku-0.0.9/haiku/_src/nets/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,20 @@
     at least once.
 
     The contract of reverse is that the reversed module will accept the output
     of the parent module as input and produce an output which is the input size
     of the parent.
 
     >>> mlp = hk.nets.MLP([1, 2, 3])
-    >>> y = mlp(jnp.ones([1, 2]))
+    >>> mlp_in = jnp.ones([1, 2])
+    >>> y = mlp(mlp_in)
     >>> rev = mlp.reverse()
-    >>> rev(y)
-    DeviceArray(...)
+    >>> rev_mlp_out = rev(y)
+    >>> mlp_in.shape == rev_mlp_out.shape
+    True
 
     Args:
       activate_final: Whether the final layer of the MLP should be activated.
       name: Optional name for the new module. The default name will be the name
         of the current module prefixed with ``"reversed_"``.
 
     Returns:
```

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/mlp_test.py` & `dm-haiku-0.0.9/haiku/_src/nets/mlp_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/mobilenetv1.py` & `dm-haiku-0.0.9/haiku/_src/nets/mobilenetv1.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/mobilenetv1_test.py` & `dm-haiku-0.0.9/haiku/_src/nets/mobilenetv1_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/resnet.py` & `dm-haiku-0.0.9/haiku/_src/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/resnet_test.py` & `dm-haiku-0.0.9/haiku/_src/nets/resnet_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/vqvae.py` & `dm-haiku-0.0.9/haiku/_src/nets/vqvae.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/nets/vqvae_test.py` & `dm-haiku-0.0.9/haiku/_src/nets/vqvae_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/pad.py` & `dm-haiku-0.0.9/haiku/_src/pad.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/pad_test.py` & `dm-haiku-0.0.9/haiku/_src/pad_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/pool.py` & `dm-haiku-0.0.9/haiku/_src/pool.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/pool_test.py` & `dm-haiku-0.0.9/haiku/_src/pool_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/random.py` & `dm-haiku-0.0.9/haiku/_src/random.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/random_test.py` & `dm-haiku-0.0.9/haiku/_src/random_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/recurrent.py` & `dm-haiku-0.0.9/haiku/_src/recurrent.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/recurrent_test.py` & `dm-haiku-0.0.9/haiku/_src/recurrent_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/reshape.py` & `dm-haiku-0.0.9/haiku/_src/reshape.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/reshape_test.py` & `dm-haiku-0.0.9/haiku/_src/reshape_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/rms_norm.py` & `dm-haiku-0.0.9/haiku/_src/rms_norm.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,53 +19,63 @@
 
 from collections import abc
 import types
 from typing import Optional, Sequence, Union
 
 from haiku._src import base
 from haiku._src import initializers
+from haiku._src import layer_norm
 from haiku._src import module
 import jax
 import jax.numpy as jnp
 
 # If you are forking replace this with `import haiku as hk`.
 hk = types.ModuleType("haiku")
 hk.get_parameter = base.get_parameter
 hk.initializers = initializers
 hk.Module = module.Module
 del base, module, initializers
 
+AxisOrAxes = Union[int, Sequence[int], slice]
+
 
 class RMSNorm(hk.Module):
   """RMSNorm module.
 
   RMSNorm provides an alternative that can be both faster and more stable than
   LayerNorm. The inputs are normalized by the root-mean-squared (RMS) and scaled
   by a learned parameter, but they are not recentered around their mean.
 
   See https://arxiv.org/pdf/1910.07467.pdf
   """
 
   def __init__(
       self,
-      axis: Union[int, Sequence[int], slice],
+      axis: AxisOrAxes,
       eps: float = 1e-5,
       scale_init: Optional[hk.initializers.Initializer] = None,
       name: Optional[str] = None,
-      create_scale: bool = True):
+      create_scale: bool = True,
+      *,
+      param_axis: Optional[AxisOrAxes] = None,
+      ):
     """Constructs a RMSNorm module.
 
     Args:
       axis: Integer, list of integers, or slice indicating which axes to
         normalize over.
       eps: Small epsilon to avoid division by zero variance. Defaults to 1e-5.
       scale_init: Optional initializer for gain (aka scale). By default, one.
       name: The module name.
       create_scale: Bool, defines whether to create a trainable scale
         per channel applied after the normalization.
+      param_axis: Axis used to determine the parameter shape of the learnable
+        scale/offset. Sonnet sets this to the channel/feature axis (e.g. to
+        ``-1`` for ``NHWC``). Other libraries set this to the same as the
+        reduction axis (e.g. ``axis=param_axis``). `None` defaults to (-1,).
     """
     super().__init__(name=name)
     if not create_scale and scale_init is not None:
       raise ValueError("Cannot set `scale_init` if `create_scale=False`.")
     if isinstance(axis, slice):
       self.axis = axis
     elif isinstance(axis, int):
@@ -75,31 +85,44 @@
       self.axis = tuple(axis)
     else:
       raise ValueError("`axis` should be an int, slice or iterable of ints.")
 
     self.eps = eps
     self.create_scale = create_scale
     self.scale_init = scale_init or jnp.ones
+    if param_axis is None:
+      self.param_axis = (-1,)
+    else:
+      self.param_axis = layer_norm.to_axes_or_slice(param_axis)
 
   def __call__(self, inputs: jnp.ndarray):
     """Connects the layer norm.
 
     Args:
       inputs: An array, where the data format is ``[N, ..., C]``.
 
     Returns:
       The normalized array, of the same shape as the inputs.
     """
     axis = self.axis
     if isinstance(axis, slice):
       axis = tuple(range(inputs.ndim)[axis])
 
+    param_axis = layer_norm.to_abs_axes(self.param_axis, inputs.ndim)
+    if param_axis == (inputs.ndim - 1,):
+      # For param_axis=-1 we store non-broadcast param shape for compatibility
+      # with older checkpoints.
+      param_shape = inputs.shape[-1:]
+    else:
+      param_shape = tuple(
+          (inputs.shape[i] if i in param_axis else 1)
+          for i in range(inputs.ndim))
     if self.create_scale:
-      scale = hk.get_parameter("scale", inputs.shape[-1:], inputs.dtype,
-                               init=self.scale_init)
+      scale = hk.get_parameter(
+          "scale", param_shape, inputs.dtype, init=self.scale_init)
       scale = jnp.broadcast_to(scale, inputs.shape)
     else:
       scale = 1.
 
     mean_squared = jnp.mean(jnp.square(inputs), axis=axis, keepdims=True)
     mean_squared = jnp.broadcast_to(mean_squared, inputs.shape)
```

### Comparing `dm-haiku-0.0.8/haiku/_src/spectral_norm.py` & `dm-haiku-0.0.9/haiku/_src/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/spectral_norm_test.py` & `dm-haiku-0.0.9/haiku/_src/spectral_norm_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/stateful.py` & `dm-haiku-0.0.9/haiku/_src/stateful.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Wrappers for JAX transformations that respect Haiku internal state."""
 
 import collections
+import collections.abc
 import functools
 import inspect
 from typing import Any, Callable, Mapping, MutableMapping, Optional, Tuple, TypeVar
 
 from haiku._src import base
 import jax
 import jax.numpy as jnp
@@ -109,16 +110,16 @@
   ...   m = MyModule()
   ...   g = hk.grad(m)(x)
   ...   return g
 
   >>> f = hk.transform_with_state(f)
   >>> x = jnp.array(2.)
   >>> params, state = jax.jit(f.init)(None, x)
-  >>> state["my_module"]["last"]
-  DeviceArray(4., dtype=float32, weak_type=True)
+  >>> print(state["my_module"]["last"])
+  4.0
 
   Args:
     fun: Function to be differentiated. Its arguments at positions specified by
       ``argnums`` should be arrays, scalars, or standard Python containers. It
       should return a scalar (which includes arrays with shape ``()`` but not
       arrays with shape ``(1,)`` etc.)
     argnums: Optional, integer or tuple of integers. Specifies which positional
@@ -730,14 +731,16 @@
                         "`hk.vmap.require_split_rng = False`.") from e
 
     return f(*args, **kwargs)
 
   wrapper.require_split_rng = True
   return wrapper
 
+list_to_tuple = lambda x: tuple(x) if isinstance(x, list) else x
+
 
 @add_split_rng_error
 def vmap(
     fun: Callable[..., Any],
     in_axes=0,
     out_axes=0,
     axis_name: Optional[str] = None,
@@ -789,15 +792,15 @@
         f"{fun.__name__} must have at least one non-None value in in_axes "
         "to use with `hk.vmap`.")
 
   # TODO(tomhennigan): Allow configuration of params/state mapping.
   params_axes = state_axes = None
   rng_axes = (0 if split_rng else None)
   haiku_state_axes = InternalState(params_axes, state_axes, rng_axes)
-  in_axes = in_axes, haiku_state_axes
+  in_axes = list_to_tuple(in_axes), haiku_state_axes
   out_axes = out_axes, haiku_state_axes
 
   @functools.wraps(fun)
   def pure_fun(args, state_in):
     if split_rng:
       # NOTE: In the case of split_rng we recieve an RNG key (rather than the
       # internal state of a PRNGSequence) so we need to construct that here.
@@ -825,15 +828,15 @@
       state = internal_state()  # Needed since we mutated internal RNG.
       saved_rng = state.rng
       state = InternalState(state.params, state.state, rng)
 
     try:
       out, state = mapped_pure_fun(args, state)
     except ValueError as err:
-      if "out_axes" in str(err):
+      if split_rng and not base.params_frozen() and "out_axes" in str(err):
         # TODO(lenamartens): add error for state too.
         raise ValueError("hk.vmap does not support setting split_rng to True "
                          "during initialization because it assumes parameters "
                          "are always shared along the mapped dimension. "
                          "Consider switching the value of `split_rng` to False "
                          "during initialization through "
                          "`split_rng=(not hk.running_init())`."
@@ -882,17 +885,19 @@
 
   @functools.wraps(body_fun)
   def pure_body_fun(val):
     val, state = val
     with temporary_internal_state(state), \
          base.push_jax_trace_level():
       val = body_fun(val)
+      reserve_up_to_full_rng_block()
       state = internal_state()
       return val, state
 
+  reserve_up_to_full_rng_block()
   init_val = (init_val, internal_state())
   val, state = jax.lax.while_loop(pure_cond_fun, pure_body_fun, init_val)
   update_internal_state(state)
   return val
 
 
 def named_call(
@@ -920,33 +925,15 @@
       side_channel["non_jaxtypes"] = non_jaxtypes
       side_channel["treedef"] = treedef
       return jax_types
     return named_call_hidden_outputs
 
   @functools.wraps(fun)
   def wrapper(*args, **kwargs):
-    if jax.config.jax_experimental_name_stack:
-      return jax.named_call(fun, name=name)(*args, **kwargs)
-
-    side_channel = {"non_jaxtypes": [], "treedef": None}
-    wrapped_fun = hide_non_jaxtype_outputs(fun, side_channel)
-    if base.inside_transform():
-      wrapped_fun = thread_hk_state_in_kwargs(jax.named_call)(wrapped_fun,
-                                                              name=name)
-    else:
-      wrapped_fun = jax.named_call(wrapped_fun, name=name)
-
-    jax_types = wrapped_fun(*args, **kwargs)
-
-    non_jaxtypes = side_channel["non_jaxtypes"]
-    out_leaves = [y if x is None else x
-                  for x, y in zip(jax_types, non_jaxtypes)]
-    out = jax.tree_util.tree_unflatten(side_channel["treedef"], out_leaves)
-
-    return out
+    return jax.named_call(fun, name=name)(*args, **kwargs)
   return wrapper
 
 
 def eval_shape(fun, *args, **kwargs):
   """Equivalent to jax.eval_shape with any changed Haiku state discarded."""
   if not base.inside_transform():
     raise ValueError(
```

### Comparing `dm-haiku-0.0.8/haiku/_src/stateful_test.py` & `dm-haiku-0.0.9/haiku/_src/stateful_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,14 +518,27 @@
       return i
 
     base.reserve_rng_keys(5)
     branches = [lambda _, i=i: branch_f(i) for i in range(5)]
     self.assertEqual(stateful.switch(3, branches, None), 3)
     self.assertEqual(stateful.switch(0, branches, None), 0)
 
+  @test_utils.transform_and_run
+  def test_stateful_while_loop_with_rng_use(self):
+    def body_fun(i):
+      _ = base.next_rng_key()
+      _ = base.next_rng_key()
+      return i+1
+
+    base.reserve_rng_keys(5)
+    if transform.running_init():
+      body_fun(0)
+    else:
+      stateful.while_loop(lambda i: i < 7, body_fun, 0)  # does not crash.
+
   @parameterized.parameters(*it.product((0, 1, 2, 4, 8), (1, 2, 3)))
   @test_utils.transform_and_run
   def test_fori(self, lower, n):
     upper = lower + n
     m = CountingModule()
     y = stateful.fori_loop(lower, upper, lambda i, x: m(i), 2)
     self.assertEqual(y, jnp.square(upper - 1))
@@ -588,14 +601,20 @@
   def test_vmap_in_axes_different_size(self):
     x = jnp.ones([1, 2])
     with self.assertRaisesRegex(
         ValueError, "vmap got inconsistent sizes for array axes to be mapped"):
       stateful.vmap(lambda a, b: None, in_axes=(0, 1), split_rng=False)(x, x)
 
   @test_utils.transform_and_run
+  def test_vmap_in_axes_supports_list(self):
+    a = jnp.ones([4])
+    b = stateful.vmap(lambda a: a * 2, in_axes=[0], split_rng=False)(a)
+    np.testing.assert_array_equal(b, a * 2)
+
+  @test_utils.transform_and_run
   def test_vmap_no_split_rng(self):
     key_before = base.next_rng_key()
     f = stateful.vmap(lambda _: base.next_rng_key(), split_rng=False)
     x = jnp.arange(4)
     k1, k2, k3, k4 = f(x)
     key_after = base.next_rng_key()
     np.testing.assert_array_equal(k1, k2)
@@ -628,14 +647,35 @@
                          init=initializers.TruncatedNormal())
     f = stateful.vmap(creates_params, split_rng=True)
     x = jnp.arange(4)
     with self.assertRaisesRegex(ValueError,
                                 "split_rng to True during initialization"):
       f(x)
 
+  @test_utils.transform_and_run(run_apply=False)
+  def test_vmap_split_rng_out_axes_error_no_split_rng(self):
+    f = stateful.vmap(lambda x: x, split_rng=False, out_axes=None)
+    x = jnp.arange(4)
+    with self.assertRaisesRegex(ValueError,
+                                "vmap has mapped output but out_axes is None"):
+      # test our split_rng error does not clobber jax error message.
+      f(x)
+
+  def test_vmap_split_rng_out_axes_error_no_init(self):
+    @transform.transform
+    def g(x):
+      f = stateful.vmap(lambda x: x, split_rng=True, out_axes=None)
+      f(x)
+
+    x = jnp.arange(4)
+    with self.assertRaisesRegex(ValueError,
+                                "vmap has mapped output but out_axes is None"):
+      # test our split_rng error does not clobber jax error message.
+      g.apply({}, jax.random.PRNGKey(42), x)
+
   def test_while_loop_rejected_in_init(self):
     def f():
       stateful.while_loop(lambda x: x.all(), lambda x: not x, 1)
     f = transform.transform(f)
     with self.assertRaisesRegex(
         ValueError, "hk.while_loop does not support initialization"):
       f.init(None)
```

### Comparing `dm-haiku-0.0.8/haiku/_src/summarise.py` & `dm-haiku-0.0.9/haiku/_src/summarise.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/summarise_test.py` & `dm-haiku-0.0.9/haiku/_src/summarise_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/test_utils.py` & `dm-haiku-0.0.9/haiku/_src/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
   ...     out = f(jnp.ones([1, 1]))
   ...     self.assertEqual(out.ndim, 2)
 
   And can also be useful in an interactive environment like ipython, Jupyter or
   Google Colaboratory:
 
   >>> f = lambda x: hk.Bias()(x)
-  >>> hk.testing.transform_and_run(f)(jnp.ones([1, 1]))
-  DeviceArray([[1.]], dtype=float32)
+  >>> print(hk.testing.transform_and_run(f)(jnp.ones([1, 1])))
+  [[1.]]
 
   See :func:`transform` for more details.
 
   To use this with `pmap` (without ``chex``) you need to additionally pass in a
   function to map the init/apply rng keys. For example, if you want every
   instance of your pmap to have the same key:
```

### Comparing `dm-haiku-0.0.8/haiku/_src/test_utils_test.py` & `dm-haiku-0.0.9/haiku/_src/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/transform.py` & `dm-haiku-0.0.9/haiku/_src/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,16 @@
   >>> def f(x):
   ...   mod = hk.Linear(10)
   ...   return mod(x)
   >>> f = hk.without_state(hk.transform_with_state(f))
   >>> rng = jax.random.PRNGKey(42)
   >>> x = jnp.zeros([1, 1])
   >>> params = f.init(rng, x)
-  >>> f.apply(params, rng, x)
-  DeviceArray([[0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]], dtype=float32)
+  >>> print(f.apply(params, rng, x))
+  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]]
 
   Args:
     f: A transformed function.
 
   Returns:
     A transformed function that does not take or return state.
   """
@@ -147,16 +147,16 @@
   >>> f = hk.with_empty_state(hk.transform(f))
   >>> rng = jax.random.PRNGKey(42)
   >>> x = jnp.zeros([1, 1])
   >>> params, state = f.init(rng, x)
   >>> state
   {}
   >>> out, state = f.apply(params, state, rng, x)
-  >>> out
-  DeviceArray([[0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]], dtype=float32)
+  >>> print(out)
+  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]]
   >>> state
   {}
 
   Args:
     f: A transformed function.
 
   Returns:
@@ -213,32 +213,32 @@
   ...   return a(x) + b(x)
   >>> f = hk.transform(f)
 
   To get the initial state of the module call ``init`` with an example input:
 
   >>> params = f.init(None, 1)
   >>> params
-  {'my_module': {'w': DeviceArray(0., dtype=float32)},
-   'my_module_1': {'w': DeviceArray(0., dtype=float32)}}
+  {'my_module': {'w': ...Array(0., dtype=float32)},
+   'my_module_1': {'w': ...Array(0., dtype=float32)}}
 
   You can then apply the function with the given parameters by calling
   ``apply`` (note that since we don't use Haiku's random number APIs to apply
   our network we pass ``None`` as an RNG key):
 
-  >>> f.apply(params, None, 1)
-  DeviceArray(2., dtype=float32)
+  >>> print(f.apply(params, None, 1))
+  2.0
 
   It is expected that your program will at some point produce updated parameters
   and you will want to re-apply ``apply``. You can do this by calling ``apply``
   with different parameters:
 
   >>> new_params = {"my_module": {"w": jnp.array(2.)},
   ...               "my_module_1": {"w": jnp.array(3.)}}
-  >>> f.apply(new_params, None, 2)
-  DeviceArray(9., dtype=float32, weak_type=True)
+  >>> print(f.apply(new_params, None, 2))
+  9.0
 
   If your transformed function needs to maintain internal state (e.g. moving
   averages in batch norm) then see :func:`transform_with_state`.
 
   Args:
     f: A function closing over :class:`Module` instances.
     apply_rng: In the process of being removed. Can only value `True`.
@@ -300,16 +300,16 @@
   ...   hk.set_state("counter", counter + 1)
   ...   return counter
   >>> f = hk.transform_with_state(f)
 
   >>> params, state = f.init(None)
   >>> for _ in range(10):
   ...   counter, state = f.apply(params, state, None)
-  >>> counter
-  DeviceArray(9, dtype=int32)
+  >>> print(counter)
+  9
 
   Args:
     f: A function closing over :class:`Module` instances.
 
   Returns:
     A :class:`TransformedWithState` tuple with ``init`` and ``apply`` pure
     functions.
```

### Comparing `dm-haiku-0.0.8/haiku/_src/transform_test.py` & `dm-haiku-0.0.9/haiku/_src/transform_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/typing.py` & `dm-haiku-0.0.9/haiku/_src/typing.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/typing_test.py` & `dm-haiku-0.0.9/haiku/_src/typing_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/_src/utils.py` & `dm-haiku-0.0.9/haiku/_src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Misc utility functions."""
 
-import collections
+import collections.abc
 import decimal
 import inspect
 import pprint
 import re
 from typing import Any, Sequence, Tuple, Type, TypeVar, Union
 
 import jax
```

### Comparing `dm-haiku-0.0.8/haiku/_src/utils_test.py` & `dm-haiku-0.0.9/haiku/_src/utils_test.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/benchmarks/eval_shape.py` & `dm-haiku-0.0.9/haiku/benchmarks/eval_shape.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/benchmarks/init.py` & `dm-haiku-0.0.9/haiku/benchmarks/init.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/config.py` & `dm-haiku-0.0.9/haiku/config.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/data_structures.py` & `dm-haiku-0.0.9/haiku/data_structures.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/experimental/__init__.py` & `dm-haiku-0.0.9/haiku/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/experimental/jaxpr_info.py` & `dm-haiku-0.0.9/haiku/experimental/jaxpr_info.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/initializers.py` & `dm-haiku-0.0.9/haiku/initializers.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/mixed_precision.py` & `dm-haiku-0.0.9/haiku/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/nets.py` & `dm-haiku-0.0.9/haiku/nets.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/pad.py` & `dm-haiku-0.0.9/haiku/pad.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/testing.py` & `dm-haiku-0.0.9/haiku/testing.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/haiku/typing.py` & `dm-haiku-0.0.9/haiku/typing.py`

 * *Files identical despite different names*

### Comparing `dm-haiku-0.0.8/setup.py` & `dm-haiku-0.0.9/setup.py`

 * *Files identical despite different names*

