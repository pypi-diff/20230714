# Comparing `tmp/fedml-0.8.7a3.tar.gz` & `tmp/fedml-0.8.7a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fedml-0.8.7a3.tar", last modified: Fri Jul 14 11:34:14 2023, max compression
+gzip compressed data, was "dist/fedml-0.8.7a4.tar", last modified: Fri Jul 14 19:14:20 2023, max compression
```

## Comparing `fedml-0.8.7a3.tar` & `fedml-0.8.7a4.tar`

### file list

```diff
@@ -1,1187 +1,1187 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/
--rw-r--r--   0 runner     (501) staff       (20)     3806 2023-07-14 11:34:14.000000 fedml-0.8.7a3/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/tests/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/tests/security/attack/
--rw-r--r--   0 runner     (501) staff       (20)     2718 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_label_flipping_attack.py
--rw-r--r--   0 runner     (501) staff       (20)      730 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_backdoor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1159 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_model_replacement_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5147 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_invertgradient.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_byzantine_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5519 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1091 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_edge_case_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     1466 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/attack/test_dlg.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/tests/security/defense/
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_rfa.py
--rw-r--r--   0 runner     (501) staff       (20)     1942 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_residual_based_reweighting.py
--rw-r--r--   0 runner     (501) staff       (20)     1139 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_wbc.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1099 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_crfl.py
--rw-r--r--   0 runner     (501) staff       (20)     1889 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_geometric_median.py
--rw-r--r--   0 runner     (501) staff       (20)     2682 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_slsgd_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1327 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_weak_dp.py
--rw-r--r--   0 runner     (501) staff       (20)     1525 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_norm_diff_clipping.py
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1555 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_bulyan.py
--rw-r--r--   0 runner     (501) staff       (20)      805 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_robust_learning_rate_defense.py
--rw-r--r--   0 runner     (501) staff       (20)      999 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_coordinate_wise_trimmed_mean.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1206 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_krum.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1276 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_cclip.py
--rw-r--r--   0 runner     (501) staff       (20)      408 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_coordinate_median.py
--rw-r--r--   0 runner     (501) staff       (20)      902 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_foolsgold_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2208 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/security/defense/test_soteria.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2326 2023-07-14 11:33:50.000000 fedml-0.8.7a3/README.md
--rw-r--r--   0 runner     (501) staff       (20)     4554 2023-07-14 11:33:53.000000 fedml-0.8.7a3/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2026 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       89 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       89 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2003 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2024 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)     4403 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)     5218 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2033 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
--rw-r--r--   0 runner     (501) staff       (20)     2020 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1435 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2119 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)     4098 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1739 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py
--rw-r--r--   0 runner     (501) staff       (20)     5323 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1999 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2013 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/trpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2003 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1993 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py
--rw-r--r--   0 runner     (501) staff       (20)     3354 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1387 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)     2007 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
--rw-r--r--   0 runner     (501) staff       (20)      699 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/privacy/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/privacy/mpi_fedavg_dp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mpi_fedavg_dp_mnist_lr_example/cross_silo_with_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mpi_fedavg_dp_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      965 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      966 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      966 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)      966 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_device/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/
--rw-r--r--   0 runner     (501) staff       (20)     1214 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      801 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/
--rw-r--r--   0 runner     (501) staff       (20)     1178 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3268 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/centralized/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/centralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    20282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/centralized/main.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_fedopt_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_fedopt_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_fedopt_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_vertical_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_vertical_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_fedopt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedopt_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedopt_mnist_lr_example/torch_fedopt_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_decentralized_fl_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_decentralized_fl_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      222 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_decentralized_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_decentralized_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_decentralized_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/torch_fedgkt_cifar10_resnet56.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     5590 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     4816 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/reddit_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6461 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/main.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_hierarchicalfl_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_hierarchicalfl_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_hierarchicalfl_mnist_lr_example/torch_hierarchicalfl_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedopt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedopt_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedopt_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedgan_mnist_gan_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedgan_mnist_gan_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedgan_mnist_gan_example/torch_fedgan_mnist_gan_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_fedavg_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_seq/
--rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_seq/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_fedprox_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_fedprox_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_fedprox_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fednas_cifar10_dart_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fednas_cifar10_dart_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fednas_cifar10_dart_example/torch_fednas_cifar10_dart_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/torch_splitnn_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_fednova_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fednova_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fednova_mnist_lr_example/torch_fednova_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_base_framework_example/
--rw-r--r--   0 runner     (501) staff       (20)      222 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_base_framework_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_cnn_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_cnn_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_cnn_example/torch_fedavg_mnist_cnn_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedprox_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedprox_mnist_lr_example/torch_fedprox_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_fedprox_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_turboaggregate_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_async_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_async_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1042 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_datasets_and_models_example/torch_fedavg_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/examples/simulation/sp_fedavg_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/intersection_and_cardinality_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/intersection_and_cardinality_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/intersection_and_cardinality_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/intersection_and_cardinality_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/heavy_hitter_twitter_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/heavy_hitter_twitter_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/heavy_hitter_twitter_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/heavy_hitter_twitter_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/frequency_estimation_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/frequency_estimation_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/frequency_estimation_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/frequency_estimation_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/avg_self_defined_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      316 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/avg_self_defined_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      280 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/avg_self_defined_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/avg_self_defined_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/avg_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      316 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/avg_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/avg_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/avg_fake_data_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/k_percentile_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/k_percentile_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/k_percentile_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/k_percentile_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/examples/federated_analytics/union_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/union_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/union_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:51.000000 fedml-0.8.7a3/examples/federated_analytics/union_fake_data_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-14 11:34:14.000000 fedml-0.8.7a3/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/
--rw-r--r--   0 runner     (501) staff       (20)     1061 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/launch_serving.py
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/launch_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)     7392 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/runner.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cross_silo/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/
--rw-r--r--   0 runner     (501) staff       (20)     3009 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_message_define.py
--rw-r--r--   0 runner     (501) staff       (20)    11077 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13517 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)    12846 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     3467 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_api.py
--rw-r--r--   0 runner     (501) staff       (20)      157 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cross_silo/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15928 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11720 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1917 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2025 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cross_silo/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     8064 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_silo/client/fedml_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     1079 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/launch_cross_silo_horizontal.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/serving/
--rw-r--r--   0 runner     (501) staff       (20)      163 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/serving/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15566 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11613 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1340 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1456 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/serving/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7549 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/serving/client/fedml_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/schedule/
--rw-r--r--   0 runner     (501) staff       (20)     5761 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/schedule/runtime_estimate.py
--rw-r--r--   0 runner     (501) staff       (20)     9840 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/schedule/seq_train_scheduler.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/schedule/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/alg_frame/
--rw-r--r--   0 runner     (501) staff       (20)      795 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/alg_frame/params.py
--rw-r--r--   0 runner     (501) staff       (20)     2349 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/alg_frame/client_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/alg_frame/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      894 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/alg_frame/context.py
--rw-r--r--   0 runner     (501) staff       (20)     5792 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/alg_frame/server_aggregator.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/topology/
--rw-r--r--   0 runner     (501) staff       (20)     5001 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/topology/asymmetric_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      479 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/topology/base_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     3853 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/topology/symmetric_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/topology/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/crypto/
--rw-r--r--   0 runner     (501) staff       (20)     2167 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/crypto/crypto_api.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/crypto/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8764 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/fedml_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/observer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/s3/
--rw-r--r--   0 runner     (501) staff       (20)     1680 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/s3/remote_storage_mnn.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/s3/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22460 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/s3/remote_storage.py
--rw-r--r--   0 runner     (501) staff       (20)     2792 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/s3/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mpi/
--rw-r--r--   0 runner     (501) staff       (20)     1648 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mpi/mpi_send_thread.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mpi/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4977 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mpi/com_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1603 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mpi/mpi_receive_thread.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_server.py
--rw-r--r--   0 runner     (501) staff       (20)     6381 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/proto/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/proto/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4236 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/ip_config_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     6272 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/trpc/
--rw-r--r--   0 runner     (501) staff       (20)     1614 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/trpc/trpc_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/trpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4807 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/trpc/trpc_comm_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/trpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      377 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2612 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/message.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_web3/
--rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_web3/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14594 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_thetastore/
--rwxr-xr-x   0 runner     (501) staff       (20)      109 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_thetastore/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14669 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)      869 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      518 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/base_com_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3/
--rwxr-xr-x   0 runner     (501) staff       (20)      123 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    15504 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    14081 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt/mqtt_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3_mnn/
--rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3_mnn/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    12233 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/web3_storage/
--rw-r--r--   0 runner     (501) staff       (20)     3604 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/web3_storage/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/theta_storage/
--rw-r--r--   0 runner     (501) staff       (20)     6834 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/theta_storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/distributed_storage/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/distributed/flow/
--rw-r--r--   0 runner     (501) staff       (20)    12684 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/flow/fedml_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/flow/fedml_executor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/flow/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      338 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/flow/fedml_flow_constants.py
--rw-r--r--   0 runner     (501) staff       (20)     3248 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/distributed/flow/test_fedml_flow.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/security/attack/
--rw-r--r--   0 runner     (501) staff       (20)     4005 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/model_replacement_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)      696 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/attack_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3424 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/edge_case_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     3607 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/byzantine_attack.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6102 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/lazy_worker.py
--rw-r--r--   0 runner     (501) staff       (20)    27345 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/invert_gradient_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     6112 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/dlg_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     4712 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/revealing_labels_from_gradients_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     3928 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/label_flipping_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5286 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/attack/backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     4414 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/fedml_attacker.py
--rw-r--r--   0 runner     (501) staff       (20)     1278 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7879 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/fedml_defender.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/security/common/
--rw-r--r--   0 runner     (501) staff       (20)     2016 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/common/bucket.py
--rw-r--r--   0 runner     (501) staff       (20)      734 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/common/net.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1875 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/common/attack_defense_data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     8805 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/common/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/security/defense/
--rw-r--r--   0 runner     (501) staff       (20)     8885 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/three_sigma_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2148 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/norm_diff_clipping_defense.py
--rw-r--r--   0 runner     (501) staff       (20)    10054 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/residual_based_reweighting_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     8375 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/three_sigma_krum_defense.py
--rw-r--r--   0 runner     (501) staff       (20)      994 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2849 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/slsgd_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1629 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/coordinate_wise_median_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3640 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/wbc_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2675 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/robust_learning_rate_defense.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1071 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/RFA_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1682 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/defense_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3568 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/foolsgold_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3709 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/soteria_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     5462 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/bulyan_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     4636 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/cross_round_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     6525 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/three_sigma_geomedian_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2022 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/geometric_median_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3320 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/crfl_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1173 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/outlier_detection.py
--rw-r--r--   0 runner     (501) staff       (20)     1008 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/weak_dp_defense.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2876 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/cclip_defense.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2564 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/security/defense/krum_defense.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/mlops/
--rw-r--r--   0 runner     (501) staff       (20)    12079 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_configs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/mlops/ssl/
--rw-r--r--   0 runner     (501) staff       (20)     4089 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)     4085 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)     1947 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/ssl/open-root-ca.crt
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/ssl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4093 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)    21364 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_metrics.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_profiler_event.py
--rw-r--r--   0 runner     (501) staff       (20)     1377 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_status.py
--rw-r--r--   0 runner     (501) staff       (20)    35246 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11124 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/stats_impl.py
--rw-r--r--   0 runner     (501) staff       (20)     1747 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    18085 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_runtime_log_daemon.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4121 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/system_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     8514 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mlops/mlops_runtime_log.py
--rw-r--r--   0 runner     (501) staff       (20)     1117 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/common/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      298 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/common/ml_engine_backend.py
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/common/singleton.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/mpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6017 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mpc/lightsecagg.py
--rw-r--r--   0 runner     (501) staff       (20)    12340 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/mpc/secagg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/dp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/dp/mechanisms/
--rw-r--r--   0 runner     (501) staff       (20)     1443 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/mechanisms/dp_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/mechanisms/laplace.py
--rw-r--r--   0 runner     (501) staff       (20)       83 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/mechanisms/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      177 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/mechanisms/base_dp_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/mechanisms/gaussian.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/dp/test/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/test/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2532 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/test/test_fed_privacy_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)     4178 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/fedml_differential_privacy.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/dp/frames/
--rw-r--r--   0 runner     (501) staff       (20)     3293 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/frames/NbAFL.py
--rw-r--r--   0 runner     (501) staff       (20)     2444 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/frames/dp_clip.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/frames/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1101 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/frames/cdp.py
--rw-r--r--   0 runner     (501) staff       (20)      470 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/frames/ldp.py
--rw-r--r--   0 runner     (501) staff       (20)     2118 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/frames/base_dp_solution.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/dp/budget_accountant/
--rw-r--r--   0 runner     (501) staff       (20)     6747 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/budget_accountant/rdp_analysis.py
--rw-r--r--   0 runner     (501) staff       (20)     1141 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/budget_accountant/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6915 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/budget_accountant/rdp_accountant.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/dp/common/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/common/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2411 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/dp/common/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/contribution/
--rw-r--r--   0 runner     (501) staff       (20)     5603 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/contribution/gtg_shapley_value.py
--rw-r--r--   0 runner     (501) staff       (20)     3197 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/contribution/mr_shapley_value.py
--rw-r--r--   0 runner     (501) staff       (20)     1665 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/contribution/base_contribution_assessor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/contribution/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4930 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/contribution/leave_one_out.py
--rw-r--r--   0 runner     (501) staff       (20)     1922 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/contribution/contribution_assessor_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/core/data/
--rw-r--r--   0 runner     (501) staff       (20)      158 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4937 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/core/data/noniid_partition.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/distributed/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/distributed/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/config/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/config/simulaton_mpi/
--rw-r--r--   0 runner     (501) staff       (20)      964 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/config/simulaton_mpi/fedml_config.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/config/simulation_sp/
--rw-r--r--   0 runner     (501) staff       (20)     1091 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/config/simulation_sp/fedml_config.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)     8022 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/arguments.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/mlops/
--rw-r--r--   0 runner     (501) staff       (20)     2755 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/mlops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/launch_cheeath.py
--rw-r--r--   0 runner     (501) staff       (20)     2198 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cross_device/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/
--rw-r--r--   0 runner     (501) staff       (20)     2190 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    18860 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2772 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/utils.py
--rw-r--r--   0 runner     (501) staff       (20)    11448 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1264 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/server_mnn/server_mnn_api.py
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      579 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cross_device/mnn_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/centralized/
--rw-r--r--   0 runner     (501) staff       (20)     6588 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/centralized/centralized_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/centralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      685 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/launch_simulation.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedavg/client.py
--rw-r--r--   0 runner     (501) staff       (20)       34 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12457 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedavg/fedavg_api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/fedprox/
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedprox/client.py
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedprox/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11535 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedprox/fedprox_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7850 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/TA_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/mpc_function.py
--rw-r--r--   0 runner     (501) staff       (20)      818 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/TA_client.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/feddyn/
--rw-r--r--   0 runner     (501) staff       (20)     1916 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/feddyn/client copy.py
--rw-r--r--   0 runner     (501) staff       (20)     1941 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/feddyn/client.py
--rw-r--r--   0 runner     (501) staff       (20)       42 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/feddyn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16395 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/feddyn/feddyn_trainer copy.py
--rw-r--r--   0 runner     (501) staff       (20)    15943 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/feddyn/feddyn_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/
--rw-r--r--   0 runner     (501) staff       (20)     1355 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/client.py
--rw-r--r--   0 runner     (501) staff       (20)     3625 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/party_models.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2241 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/vfl.py
--rw-r--r--   0 runner     (501) staff       (20)    10964 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/vfl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     3887 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/
--rw-r--r--   0 runner     (501) staff       (20)     8207 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/fednova.py
--rw-r--r--   0 runner     (501) staff       (20)    12457 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/fednova_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)    10932 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/fednova_api.py
--rw-r--r--   0 runner     (501) staff       (20)     6496 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2258 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fednova/comm_helpers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/fedopt/
--rw-r--r--   0 runner     (501) staff       (20)    12255 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedopt/fedopt_api.py
--rw-r--r--   0 runner     (501) staff       (20)     1456 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedopt/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/fedopt/optrepo.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/
--rw-r--r--   0 runner     (501) staff       (20)     2133 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2391 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/group.py
--rw-r--r--   0 runner     (501) staff       (20)     4644 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/mime/
--rw-r--r--   0 runner     (501) staff       (20)     1494 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/mime/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/mime/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3192 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/mime/opt_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    13370 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/mime/mime_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/scaffold/
--rw-r--r--   0 runner     (501) staff       (20)    13466 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/scaffold/scaffold_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     2677 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/scaffold/client.py
--rw-r--r--   0 runner     (501) staff       (20)       46 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/scaffold/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/sp/decentralized/
--rw-r--r--   0 runner     (501) staff       (20)     4187 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/decentralized/decentralized_fl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     4328 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/decentralized/client_dsgd.py
--rw-r--r--   0 runner     (501) staff       (20)     5514 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/decentralized/client_pushsum.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/decentralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5741 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/sp/decentralized/topology_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/simulation/mpi/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     2689 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6818 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3602 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAvgAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2542 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4462 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAvgServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/
--rw-r--r--   0 runner     (501) staff       (20)     2589 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2338 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/SplitNNAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      591 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     1733 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3996 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2043 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/split_nn/server_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2438 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2804 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     7365 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4607 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3460 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxAPI.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/
--rw-r--r--   0 runner     (501) staff       (20)     4494 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGanServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3809 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGanAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3633 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/gan_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)      880 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2218 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGANTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     7774 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGANAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2625 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGanClientManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/
--rw-r--r--   0 runner     (501) staff       (20)    15801 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     2120 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/FedGKTAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     3165 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4940 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      671 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/message_def.py
--rw-r--r--   0 runner     (501) staff       (20)     2925 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     6492 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/
--rw-r--r--   0 runner     (501) staff       (20)      428 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1858 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1123 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/central_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     1147 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/algorithm_api.py
--rw-r--r--   0 runner     (501) staff       (20)      438 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/client_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/base_framework/central_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     3409 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4903 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3324 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     3531 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2222 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     3863 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     7993 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     4779 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4164 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)     3274 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/
--rw-r--r--   0 runner     (501) staff       (20)     5488 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3489 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    13844 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3079 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5954 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3284 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/
--rw-r--r--   0 runner     (501) staff       (20)      386 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1112 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2374 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      738 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/algorithm_api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/
--rw-r--r--   0 runner     (501) staff       (20)      504 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     7074 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2198 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1801 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     3470 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     1842 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/host_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/simulation/mpi/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/
--rw-r--r--   0 runner     (501) staff       (20)    11022 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3767 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     2295 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    10792 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)      693 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/
--rw-r--r--   0 runner     (501) staff       (20)     3490 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     5687 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3309 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4893 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)    10695 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3306 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fednova/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/
--rw-r--r--   0 runner     (501) staff       (20)     8893 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      578 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2663 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/optrepo.py
--rw-r--r--   0 runner     (501) staff       (20)     3297 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1307 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4470 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/
--rw-r--r--   0 runner     (501) staff       (20)     3300 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    12025 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1009 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     4464 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/optrepo.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1307 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5535 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/
--rw-r--r--   0 runner     (501) staff       (20)     3507 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      716 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     1927 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     6138 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/MyModelTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12406 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)    10700 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2448 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     4172 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)      205 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/simulation/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9847 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/simulation/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)    14960 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:14.000000 fedml-0.8.7a3/fedml/utils/
--rw-r--r--   0 runner     (501) staff       (20)    10317 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/utils/model_utils.py
--rw-r--r--   0 runner     (501) staff       (20)      735 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/utils/logging.py
--rw-r--r--   0 runner     (501) staff       (20)    10524 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/utils/compression.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-07-14 11:33:53.000000 fedml-0.8.7a3/fedml/utils/context.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/
--rwxr-xr-x   0 runner     (501) staff       (20)      313 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/cli_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)    17332 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)    11014 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2263 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_daemon.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5644 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/docker_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)    53261 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_runner.py
--rw-r--r--   0 runner     (501) staff       (20)    19884 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_constants.py
--rw-r--r--   0 runner     (501) staff       (20)    10779 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_diagnosis.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2846 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/client_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3126 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/edge_deployment/simulator_daemon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/model_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)     5828 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_inference.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2317 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_client_daemon.py
--rw-r--r--   0 runner     (501) staff       (20)     8771 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/modelops_configs.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_server_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)    75936 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_server_runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)    25678 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_cards.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_client_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5417 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/docker_client_login.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    16456 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_server_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)    18262 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_cache.py
--rwxr-xr-x   0 runner     (501) staff       (20)    40997 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_deployment.py
--rwxr-xr-x   0 runner     (501) staff       (20)      816 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_server_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1766 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_object.py
--rwxr-xr-x   0 runner     (501) staff       (20)    26762 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_db.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6311 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_login_entry.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14992 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_client_data_interface.py
--rw-r--r--   0 runner     (501) staff       (20)    22536 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_server_constants.py
--rwxr-xr-x   0 runner     (501) staff       (20)     8362 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_monitor.py
--rw-r--r--   0 runner     (501) staff       (20)    29071 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_client_constants.py
--rwxr-xr-x   0 runner     (501) staff       (20)    47302 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_client_runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5442 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/docker_server_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2979 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_server_daemon.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6722 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_client_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2766 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_msg_object.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2906 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/model_deployment/device_model_inference_entry.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/env/
--rw-r--r--   0 runner     (501) staff       (20)     3453 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/env/collect_env.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/env/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    45651 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/cli.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      629 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/torch_client.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      650 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/comm_utils/
--rw-r--r--   0 runner     (501) staff       (20)    25615 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/comm_utils/sys_utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/comm_utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      295 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/comm_utils/yaml_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/server_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)      749 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/server_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)    71302 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/server_runner.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2848 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/job_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5677 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/docker_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1971 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/server_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)    10533 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/app_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2519 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/server_daemon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cli/server_deployment/templates/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/templates/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/templates/fedml-aggregator-data-pv.yaml
--rw-r--r--   0 runner     (501) staff       (20)      279 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/templates/fedml-aggregator-data-pvc.yaml
--rw-r--r--   0 runner     (501) staff       (20)      275 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/templates/fedml-server-svc.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1841 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)    13871 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/server_login.py
--rw-r--r--   0 runner     (501) staff       (20)    18216 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cli/server_deployment/server_constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cheetah/
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cheetah/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15566 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11613 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1939 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2047 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/cheetah/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7549 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/cheetah/client/fedml_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/ml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/ml/aggregator/
--rw-r--r--   0 runner     (501) staff       (20)      548 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/aggregator_creator.py
--rw-r--r--   0 runner     (501) staff       (20)     2488 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     4187 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/default_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5621 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2408 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator_classification.py
--rw-r--r--   0 runner     (501) staff       (20)    10546 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/agg_operator.py
--rw-r--r--   0 runner     (501) staff       (20)     3388 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/ml/engine/
--rw-r--r--   0 runner     (501) staff       (20)    11333 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/engine/ml_engine_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/engine/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1345 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/engine/torch_process_group_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/ml/trainer/
--rw-r--r--   0 runner     (501) staff       (20)     3953 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/scaffold_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)      580 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/trainer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)     9496 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/fednova_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/local_optimizer.py
--rw-r--r--   0 runner     (501) staff       (20)     5923 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/fedprox_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     3578 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     6857 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/feddyn_trainer copy.py
--rw-r--r--   0 runner     (501) staff       (20)     5180 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/feddyn_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5063 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     6274 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/mime_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4026 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer_tag_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)     5805 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/linear/
--rw-r--r--   0 runner     (501) staff       (20)      433 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/linear/lr.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/linear/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      544 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/linear/lr_cifar10.py
--rw-r--r--   0 runner     (501) staff       (20)       52 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4549 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/model_hub.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/mobile/
--rw-r--r--   0 runner     (501) staff       (20)      988 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/mobile/mnn_lenet.py
--rw-r--r--   0 runner     (501) staff       (20)     3860 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/mobile/mnn_resnet.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/mobile/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      774 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/mobile/torch_lenet.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/nlp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/nlp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6272 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/nlp/model_args.py
--rw-r--r--   0 runner     (501) staff       (20)     4687 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/nlp/rnn.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/finance/
--rw-r--r--   0 runner     (501) staff       (20)      458 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/finance/vfl_feature_extractor.py
--rw-r--r--   0 runner     (501) staff       (20)     2385 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/finance/vfl_models_standalone.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/finance/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      354 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/finance/vfl_classifier.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/cv/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/cv/resnet56/
--rw-r--r--   0 runner     (501) staff       (20)     9541 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet56/resnet_pretrained.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet56/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8241 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet56/resnet_server.py
--rw-r--r--   0 runner     (501) staff       (20)     9507 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet56/resnet_client.py
--rw-r--r--   0 runner     (501) staff       (20)     6216 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/vgg.py
--rw-r--r--   0 runner     (501) staff       (20)      455 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/test_cnn.py
--rw-r--r--   0 runner     (501) staff       (20)    16186 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet_torch.py
--rw-r--r--   0 runner     (501) staff       (20)    25891 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/efficientnet_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7751 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet_cifar.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10352 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/mobilenet_v3.py
--rw-r--r--   0 runner     (501) staff       (20)    19954 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/batchnorm_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7629 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/cnn.py
--rw-r--r--   0 runner     (501) staff       (20)     1590 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/mnist_gan.py
--rw-r--r--   0 runner     (501) staff       (20)    17984 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/efficientnet.py
--rw-r--r--   0 runner     (501) staff       (20)    25096 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet_all.py
--rw-r--r--   0 runner     (501) staff       (20)     4593 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/mobilenet.py
--rw-r--r--   0 runner     (501) staff       (20)    74592 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/common.py
--rw-r--r--   0 runner     (501) staff       (20)    10274 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/model/cv/darts/
--rw-r--r--   0 runner     (501) staff       (20)     7088 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/model_search_gdas.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1713 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/visualize.py
--rw-r--r--   0 runner     (501) staff       (20)    18693 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/architect.py
--rw-r--r--   0 runner     (501) staff       (20)     7681 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/model.py
--rw-r--r--   0 runner     (501) staff       (20)     4504 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/operations.py
--rw-r--r--   0 runner     (501) staff       (20)     3268 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/utils.py
--rw-r--r--   0 runner     (501) staff       (20)    12302 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/model_search.py
--rw-r--r--   0 runner     (501) staff       (20)     8673 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/train.py
--rw-r--r--   0 runner     (501) staff       (20)     3486 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/genotypes.py
--rw-r--r--   0 runner     (501) staff       (20)    14555 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/darts/train_search.py
--rw-r--r--   0 runner     (501) staff       (20)     7625 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/resnet_gn.py
--rw-r--r--   0 runner     (501) staff       (20)     5343 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/model/cv/group_normalization.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/device/
--rw-r--r--   0 runner     (501) staff       (20)     2833 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/device/gpu_mapping_cross_silo.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/device/gpu_mapping_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)     5611 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/device/device.py
--rw-r--r--   0 runner     (501) staff       (20)      112 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/device/ip_config_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/
--rw-r--r--   0 runner     (501) staff       (20)     1737 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/runner.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/cross_silo/
--rw-r--r--   0 runner     (501) staff       (20)      673 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/fa_server.py
--rw-r--r--   0 runner     (501) staff       (20)      644 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/fa_client.py
--rw-r--r--   0 runner     (501) staff       (20)      186 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/cross_silo/server/
--rw-r--r--   0 runner     (501) staff       (20)     2224 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11189 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     5262 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      879 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/server/server_initializer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/
--rw-r--r--   0 runner     (501) staff       (20)     1526 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2714 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/message_define.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2051 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/fa_local_analyzer.py
--rw-r--r--   0 runner     (501) staff       (20)     2050 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     6118 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/cross_silo/client/fedml_client_master_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/aggregator/
--rw-r--r--   0 runner     (501) staff       (20)     1903 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/frequency_estimation_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1885 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/intersection_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1559 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/union_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2114 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/avg_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3908 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/k_percentile_element_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4005 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/heavy_hitter_triehh_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/aggregator/global_analyzer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/simulation/sp/
--rw-r--r--   0 runner     (501) staff       (20)     1192 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/simulation/sp/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/simulation/sp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3449 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/simulation/sp/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)      119 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/simulation/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      606 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/simulation/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2832 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/utils/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7789 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/utils/trie.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/
--rw-r--r--   0 runner     (501) staff       (20)     1599 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/heavy_hitter_triehh.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      453 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/frequency_estimation.py
--rw-r--r--   0 runner     (501) staff       (20)     1413 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/client_analyzer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)      392 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/k_percentage_element.py
--rw-r--r--   0 runner     (501) staff       (20)      223 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/intersection.py
--rw-r--r--   0 runner     (501) staff       (20)      217 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/union.py
--rw-r--r--   0 runner     (501) staff       (20)      362 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/local_analyzer/avg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/base_frame/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/base_frame/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      716 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/base_frame/server_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1049 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/base_frame/client_analyzer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/data/
--rw-r--r--   0 runner     (501) staff       (20)     4487 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/data_loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/data/twitter_Sentiment140/
--rw-r--r--   0 runner     (501) staff       (20)     3223 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py
--rw-r--r--   0 runner     (501) staff       (20)     1693 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/twitter_Sentiment140/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/twitter_Sentiment140/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       75 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2374 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/data/self_defined_data/
--rw-r--r--   0 runner     (501) staff       (20)      856 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/self_defined_data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/self_defined_data/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/fa/data/fake_numeric_data/
--rw-r--r--   0 runner     (501) staff       (20)      526 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/fake_numeric_data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/fa/data/fake_numeric_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      545 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/launch_cross_device.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/MNIST/
--rw-r--r--   0 runner     (501) staff       (20)     5448 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/MNIST/mnist_mobile_preprocessor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4945 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/MNIST/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/MNIST/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/MNIST/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/lending_club_loan/
--rw-r--r--   0 runner     (501) staff       (20)     7729 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/lending_club_loan/lending_club_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/lending_club_loan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2291 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/lending_club_loan/lending_club_feature_group.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fed_cifar100/
--rw-r--r--   0 runner     (501) staff       (20)     6320 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_cifar100/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_cifar100/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      517 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_cifar100/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2631 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_cifar100/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/FederatedEMNIST/
--rw-r--r--   0 runner     (501) staff       (20)     6737 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/FederatedEMNIST/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/FederatedEMNIST/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      426 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/FederatedEMNIST/dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/cifar100/
--rw-r--r--   0 runner     (501) staff       (20)    11837 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar100/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2077 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar100/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar100/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    21968 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)      156 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/file_operation.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/shakespeare/
--rwxr-xr-x   0 runner     (501) staff       (20)     3431 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/shakespeare/language_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4135 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/shakespeare/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/shakespeare/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      335 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/shakespeare/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/shakespeare/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/synthetic_1_1/
--rw-r--r--   0 runner     (501) staff       (20)     4562 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/synthetic_1_1/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/synthetic_1_1/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3210 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/synthetic_1_1/stats.py
--rw-r--r--   0 runner     (501) staff       (20)     2749 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/synthetic_1_1/generate_synthetic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/Landmarks/
--rw-r--r--   0 runner     (501) staff       (20)      375 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/download_with_tff.py
--rw-r--r--   0 runner     (501) staff       (20)    14871 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/download_without_tff.py
--rw-r--r--   0 runner     (501) staff       (20)    11159 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2191 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    14342 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2090 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/check_download.py
--rw-r--r--   0 runner     (501) staff       (20)     7872 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/Landmarks/download_without_tf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fednlp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fednlp/base/
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/globals.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fednlp/base/preprocess/
--rw-r--r--   0 runner     (501) staff       (20)     4794 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/preprocess/base_example.py
--rw-r--r--   0 runner     (501) staff       (20)      363 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/preprocess/base_data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/preprocess/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      224 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/preprocess/base_preprocessor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fednlp/base/raw_data/
--rw-r--r--   0 runner     (501) staff       (20)     1428 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/raw_data/partition.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/raw_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3636 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fednlp/base/data_manager/
--rw-r--r--   0 runner     (501) staff       (20)    16505 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/data_manager/base_data_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/data_manager/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8248 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fednlp/base/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/NUS_WIDE/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/NUS_WIDE/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11281 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/NUS_WIDE/nus_wide_dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/stackoverflow_lr/
--rw-r--r--   0 runner     (501) staff       (20)     8487 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_lr/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_lr/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2841 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_lr/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     4272 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_lr/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/fed_shakespeare/
--rw-r--r--   0 runner     (501) staff       (20)     6100 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_shakespeare/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_shakespeare/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3633 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/fed_shakespeare/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/ImageNet/
--rw-r--r--   0 runner     (501) staff       (20)    11416 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/ImageNet/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     6718 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/ImageNet/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/ImageNet/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5874 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/ImageNet/datasets_hdf5.py
--rw-r--r--   0 runner     (501) staff       (20)     1429 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/data_loader_cross_silo.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/cinic10/
--rw-r--r--   0 runner     (501) staff       (20)    13807 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cinic10/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     3071 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cinic10/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cinic10/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/stackoverflow_nwp/
--rw-r--r--   0 runner     (501) staff       (20)     7023 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_nwp/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_nwp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2171 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_nwp/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2508 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/stackoverflow_nwp/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/UCI/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/UCI/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6215 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/UCI/data_loader_for_susy_and_ro.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/edge_case_examples/
--rw-r--r--   0 runner     (501) staff       (20)    44697 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/edge_case_examples/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)    20285 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/edge_case_examples/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/edge_case_examples/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml/data/cifar10/
--rw-r--r--   0 runner     (501) staff       (20)    13696 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar10/efficient_loader.py
--rw-r--r--   0 runner     (501) staff       (20)    11902 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar10/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2378 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar10/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)     3972 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar10/without_reload.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 11:33:52.000000 fedml-0.8.7a3/fedml/data/cifar10/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3806 2023-07-14 11:34:12.000000 fedml-0.8.7a3/fedml.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    48148 2023-07-14 11:34:13.000000 fedml-0.8.7a3/fedml.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)       45 2023-07-14 11:34:12.000000 fedml-0.8.7a3/fedml.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      546 2023-07-14 11:34:12.000000 fedml-0.8.7a3/fedml.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       21 2023-07-14 11:34:12.000000 fedml-0.8.7a3/fedml.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-14 11:34:12.000000 fedml-0.8.7a3/fedml.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/
+-rw-r--r--   0 runner     (501) staff       (20)     3806 2023-07-14 19:14:20.000000 fedml-0.8.7a4/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/tests/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/tests/security/attack/
+-rw-r--r--   0 runner     (501) staff       (20)     2718 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_label_flipping_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)      730 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_backdoor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_model_replacement_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_invertgradient.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_byzantine_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5519 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_edge_case_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1466 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/attack/test_dlg.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/tests/security/defense/
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_rfa.py
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_residual_based_reweighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_wbc.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1099 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_crfl.py
+-rw-r--r--   0 runner     (501) staff       (20)     1889 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_geometric_median.py
+-rw-r--r--   0 runner     (501) staff       (20)     2682 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_slsgd_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1327 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_weak_dp.py
+-rw-r--r--   0 runner     (501) staff       (20)     1525 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_norm_diff_clipping.py
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1555 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_bulyan.py
+-rw-r--r--   0 runner     (501) staff       (20)      805 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_robust_learning_rate_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)      999 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_coordinate_wise_trimmed_mean.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1206 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_krum.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1276 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_cclip.py
+-rw-r--r--   0 runner     (501) staff       (20)      408 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_coordinate_median.py
+-rw-r--r--   0 runner     (501) staff       (20)      902 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_foolsgold_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2208 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/security/defense/test_soteria.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2326 2023-07-14 19:14:04.000000 fedml-0.8.7a4/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     4554 2023-07-14 19:14:07.000000 fedml-0.8.7a4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2026 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)      196 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2003 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2024 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)     4403 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)     5218 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2033 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2020 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1435 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2119 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)     4098 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1739 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py
+-rw-r--r--   0 runner     (501) staff       (20)     5323 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1999 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2013 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/trpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2003 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1993 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     3354 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1387 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)     2007 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
+-rw-r--r--   0 runner     (501) staff       (20)      699 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/privacy/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/privacy/mpi_fedavg_dp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mpi_fedavg_dp_mnist_lr_example/cross_silo_with_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mpi_fedavg_dp_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      965 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_device/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/
+-rw-r--r--   0 runner     (501) staff       (20)     1214 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      801 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/
+-rw-r--r--   0 runner     (501) staff       (20)     1178 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3268 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/centralized/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/centralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    20282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/centralized/main.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_fedopt_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_fedopt_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_fedopt_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_vertical_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_vertical_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_fedopt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedopt_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedopt_mnist_lr_example/torch_fedopt_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_decentralized_fl_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_decentralized_fl_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_decentralized_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_decentralized_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_decentralized_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/torch_fedgkt_cifar10_resnet56.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     5590 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     4816 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/reddit_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6461 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/main.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_hierarchicalfl_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_hierarchicalfl_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_hierarchicalfl_mnist_lr_example/torch_hierarchicalfl_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedopt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedopt_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedopt_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedgan_mnist_gan_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedgan_mnist_gan_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedgan_mnist_gan_example/torch_fedgan_mnist_gan_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_fedavg_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_seq/
+-rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_seq/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_fedprox_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_fedprox_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_fedprox_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      423 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fednas_cifar10_dart_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fednas_cifar10_dart_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fednas_cifar10_dart_example/torch_fednas_cifar10_dart_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/torch_splitnn_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_fednova_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fednova_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fednova_mnist_lr_example/torch_fednova_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_base_framework_example/
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_base_framework_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_cnn_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_cnn_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_cnn_example/torch_fedavg_mnist_cnn_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedprox_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedprox_mnist_lr_example/torch_fedprox_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_fedprox_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_turboaggregate_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_async_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_async_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1042 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_datasets_and_models_example/torch_fedavg_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/examples/simulation/sp_fedavg_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/intersection_and_cardinality_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/intersection_and_cardinality_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/intersection_and_cardinality_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/intersection_and_cardinality_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/heavy_hitter_twitter_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/heavy_hitter_twitter_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/heavy_hitter_twitter_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/heavy_hitter_twitter_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/frequency_estimation_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/frequency_estimation_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/frequency_estimation_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/frequency_estimation_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/avg_self_defined_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/avg_self_defined_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      280 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/avg_self_defined_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/avg_self_defined_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/avg_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/avg_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/avg_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/avg_fake_data_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/k_percentile_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/k_percentile_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/k_percentile_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/k_percentile_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/examples/federated_analytics/union_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/union_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/union_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:06.000000 fedml-0.8.7a4/examples/federated_analytics/union_fake_data_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-14 19:14:20.000000 fedml-0.8.7a4/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/launch_serving.py
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/launch_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)     7392 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/runner.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cross_silo/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/
+-rw-r--r--   0 runner     (501) staff       (20)     3009 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)    11077 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13517 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)    12846 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3467 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_api.py
+-rw-r--r--   0 runner     (501) staff       (20)      157 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cross_silo/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15928 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11720 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1917 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2025 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cross_silo/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     8064 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_silo/client/fedml_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1079 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/launch_cross_silo_horizontal.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/serving/
+-rw-r--r--   0 runner     (501) staff       (20)      163 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/serving/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15566 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1456 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/serving/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/serving/client/fedml_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/schedule/
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/schedule/runtime_estimate.py
+-rw-r--r--   0 runner     (501) staff       (20)     9840 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/schedule/seq_train_scheduler.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/schedule/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/alg_frame/
+-rw-r--r--   0 runner     (501) staff       (20)      795 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/alg_frame/params.py
+-rw-r--r--   0 runner     (501) staff       (20)     2349 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/alg_frame/client_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/alg_frame/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      894 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/alg_frame/context.py
+-rw-r--r--   0 runner     (501) staff       (20)     5792 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/alg_frame/server_aggregator.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/topology/
+-rw-r--r--   0 runner     (501) staff       (20)     5001 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/topology/asymmetric_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      479 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/topology/base_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3853 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/topology/symmetric_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/topology/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/crypto/
+-rw-r--r--   0 runner     (501) staff       (20)     2167 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/crypto/crypto_api.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/crypto/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8764 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/fedml_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/
+-rw-r--r--   0 runner     (501) staff       (20)      153 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/observer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/s3/
+-rw-r--r--   0 runner     (501) staff       (20)     1680 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/s3/remote_storage_mnn.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/s3/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22460 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/s3/remote_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)     2792 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/s3/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mpi/
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mpi/mpi_send_thread.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mpi/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4977 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mpi/com_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mpi/mpi_receive_thread.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     6381 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/proto/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/proto/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4236 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/ip_config_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     6272 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/trpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1614 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/trpc/trpc_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/trpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4807 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/trpc/trpc_comm_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/trpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      377 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2612 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/message.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_web3/
+-rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_web3/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14594 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_thetastore/
+-rwxr-xr-x   0 runner     (501) staff       (20)      109 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_thetastore/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14669 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      869 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      518 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/base_com_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3/
+-rwxr-xr-x   0 runner     (501) staff       (20)      123 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    15504 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14081 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt/mqtt_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3_mnn/
+-rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3_mnn/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    12233 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/web3_storage/
+-rw-r--r--   0 runner     (501) staff       (20)     3604 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/web3_storage/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/theta_storage/
+-rw-r--r--   0 runner     (501) staff       (20)     6834 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/theta_storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/distributed_storage/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/distributed/flow/
+-rw-r--r--   0 runner     (501) staff       (20)    12684 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/flow/fedml_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/flow/fedml_executor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/flow/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      338 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/flow/fedml_flow_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)     3248 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/distributed/flow/test_fedml_flow.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/security/attack/
+-rw-r--r--   0 runner     (501) staff       (20)     4005 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/model_replacement_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)      696 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/attack_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3424 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/edge_case_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/byzantine_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6102 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/lazy_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)    27345 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/invert_gradient_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     6112 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/dlg_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     4712 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/revealing_labels_from_gradients_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3928 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/label_flipping_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5286 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/attack/backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     4414 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/fedml_attacker.py
+-rw-r--r--   0 runner     (501) staff       (20)     1278 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7879 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/fedml_defender.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/security/common/
+-rw-r--r--   0 runner     (501) staff       (20)     2016 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/common/bucket.py
+-rw-r--r--   0 runner     (501) staff       (20)      734 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/common/net.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1875 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/common/attack_defense_data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     8805 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/common/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/security/defense/
+-rw-r--r--   0 runner     (501) staff       (20)     8885 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/three_sigma_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2148 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/norm_diff_clipping_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)    10054 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/residual_based_reweighting_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     8375 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/three_sigma_krum_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)      994 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2849 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/slsgd_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1629 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/coordinate_wise_median_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3640 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/wbc_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2675 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/robust_learning_rate_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1071 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/RFA_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1682 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/defense_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3568 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/foolsgold_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3709 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/soteria_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     5462 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/bulyan_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     4636 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/cross_round_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     6525 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/three_sigma_geomedian_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2022 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/geometric_median_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3320 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/crfl_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/outlier_detection.py
+-rw-r--r--   0 runner     (501) staff       (20)     1008 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/weak_dp_defense.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2876 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/cclip_defense.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2564 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/security/defense/krum_defense.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/mlops/
+-rw-r--r--   0 runner     (501) staff       (20)    12079 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_configs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/mlops/ssl/
+-rw-r--r--   0 runner     (501) staff       (20)     4089 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1947 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/ssl/open-root-ca.crt
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/ssl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4093 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)    21364 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_metrics.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_profiler_event.py
+-rw-r--r--   0 runner     (501) staff       (20)     1377 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_status.py
+-rw-r--r--   0 runner     (501) staff       (20)    35246 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11124 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/stats_impl.py
+-rw-r--r--   0 runner     (501) staff       (20)     1747 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    18085 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_runtime_log_daemon.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4121 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/system_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     8514 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mlops/mlops_runtime_log.py
+-rw-r--r--   0 runner     (501) staff       (20)     1117 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/common/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/common/ml_engine_backend.py
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/common/singleton.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/mpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6017 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mpc/lightsecagg.py
+-rw-r--r--   0 runner     (501) staff       (20)    12340 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/mpc/secagg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/dp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/dp/mechanisms/
+-rw-r--r--   0 runner     (501) staff       (20)     1443 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/mechanisms/dp_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)      659 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/mechanisms/laplace.py
+-rw-r--r--   0 runner     (501) staff       (20)       83 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/mechanisms/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      177 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/mechanisms/base_dp_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/mechanisms/gaussian.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/dp/test/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/test/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2532 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/test/test_fed_privacy_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)     4178 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/fedml_differential_privacy.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/dp/frames/
+-rw-r--r--   0 runner     (501) staff       (20)     3293 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/frames/NbAFL.py
+-rw-r--r--   0 runner     (501) staff       (20)     2444 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/frames/dp_clip.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/frames/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1101 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/frames/cdp.py
+-rw-r--r--   0 runner     (501) staff       (20)      470 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/frames/ldp.py
+-rw-r--r--   0 runner     (501) staff       (20)     2118 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/frames/base_dp_solution.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/dp/budget_accountant/
+-rw-r--r--   0 runner     (501) staff       (20)     6747 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/budget_accountant/rdp_analysis.py
+-rw-r--r--   0 runner     (501) staff       (20)     1141 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/budget_accountant/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6915 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/budget_accountant/rdp_accountant.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/dp/common/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/common/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2411 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/dp/common/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/contribution/
+-rw-r--r--   0 runner     (501) staff       (20)     5603 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/contribution/gtg_shapley_value.py
+-rw-r--r--   0 runner     (501) staff       (20)     3197 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/contribution/mr_shapley_value.py
+-rw-r--r--   0 runner     (501) staff       (20)     1665 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/contribution/base_contribution_assessor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/contribution/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4930 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/contribution/leave_one_out.py
+-rw-r--r--   0 runner     (501) staff       (20)     1922 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/contribution/contribution_assessor_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/core/data/
+-rw-r--r--   0 runner     (501) staff       (20)      158 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4937 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/core/data/noniid_partition.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/distributed/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/distributed/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/config/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/config/simulaton_mpi/
+-rw-r--r--   0 runner     (501) staff       (20)      964 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/config/simulaton_mpi/fedml_config.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/config/simulation_sp/
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/config/simulation_sp/fedml_config.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)     8022 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/arguments.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/mlops/
+-rw-r--r--   0 runner     (501) staff       (20)     2755 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/mlops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/launch_cheeath.py
+-rw-r--r--   0 runner     (501) staff       (20)     2198 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cross_device/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/
+-rw-r--r--   0 runner     (501) staff       (20)     2190 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    18860 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2772 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    11448 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/server_mnn/server_mnn_api.py
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      579 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cross_device/mnn_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/centralized/
+-rw-r--r--   0 runner     (501) staff       (20)     6588 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/centralized/centralized_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/centralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      685 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/launch_simulation.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedavg/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       34 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12457 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedavg/fedavg_api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/fedprox/
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedprox/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedprox/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11535 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedprox/fedprox_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7850 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/TA_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/mpc_function.py
+-rw-r--r--   0 runner     (501) staff       (20)      818 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/TA_client.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/feddyn/
+-rw-r--r--   0 runner     (501) staff       (20)     1916 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/feddyn/client copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     1941 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/feddyn/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       42 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/feddyn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16395 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/feddyn/feddyn_trainer copy.py
+-rw-r--r--   0 runner     (501) staff       (20)    15943 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/feddyn/feddyn_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)     1355 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     3625 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/party_models.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2241 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/vfl.py
+-rw-r--r--   0 runner     (501) staff       (20)    10964 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/vfl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     3887 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/
+-rw-r--r--   0 runner     (501) staff       (20)     8207 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/fednova.py
+-rw-r--r--   0 runner     (501) staff       (20)    12457 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/fednova_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)    10932 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/fednova_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     6496 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2258 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fednova/comm_helpers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/fedopt/
+-rw-r--r--   0 runner     (501) staff       (20)    12255 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedopt/fedopt_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     1456 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedopt/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedopt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/fedopt/optrepo.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)     2133 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2391 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/group.py
+-rw-r--r--   0 runner     (501) staff       (20)     4644 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/mime/
+-rw-r--r--   0 runner     (501) staff       (20)     1494 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/mime/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/mime/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3192 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/mime/opt_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    13370 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/mime/mime_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/scaffold/
+-rw-r--r--   0 runner     (501) staff       (20)    13466 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/scaffold/scaffold_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2677 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/scaffold/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       46 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/scaffold/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/sp/decentralized/
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/decentralized/decentralized_fl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     4328 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/decentralized/client_dsgd.py
+-rw-r--r--   0 runner     (501) staff       (20)     5514 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/decentralized/client_pushsum.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/decentralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5741 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/sp/decentralized/topology_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     2689 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6818 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3602 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAvgAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2542 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4462 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAvgServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/
+-rw-r--r--   0 runner     (501) staff       (20)     2589 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2338 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/SplitNNAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     1733 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3996 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2043 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/split_nn/server_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2438 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2804 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     7365 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4607 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3460 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxAPI.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/
+-rw-r--r--   0 runner     (501) staff       (20)     4494 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGanServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3809 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGanAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/gan_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      880 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2218 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGANTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     7774 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGANAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2625 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGanClientManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/
+-rw-r--r--   0 runner     (501) staff       (20)    15801 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2120 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/FedGKTAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     3165 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4940 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      671 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/message_def.py
+-rw-r--r--   0 runner     (501) staff       (20)     2925 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6492 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/
+-rw-r--r--   0 runner     (501) staff       (20)      428 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1858 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/central_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     1147 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/algorithm_api.py
+-rw-r--r--   0 runner     (501) staff       (20)      438 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/client_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/base_framework/central_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     3409 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4903 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3324 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3531 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2222 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3863 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     7993 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     4779 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4164 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)     3274 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/
+-rw-r--r--   0 runner     (501) staff       (20)     5488 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3489 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    13844 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5954 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3284 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/
+-rw-r--r--   0 runner     (501) staff       (20)      386 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1112 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2374 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      738 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/algorithm_api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)      504 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     7074 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2198 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1801 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     3470 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1842 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/host_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/
+-rw-r--r--   0 runner     (501) staff       (20)    11022 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3767 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2295 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    10792 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      693 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/
+-rw-r--r--   0 runner     (501) staff       (20)     3490 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     5687 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3309 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4893 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)    10695 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3306 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fednova/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/
+-rw-r--r--   0 runner     (501) staff       (20)     8893 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      578 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2663 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/optrepo.py
+-rw-r--r--   0 runner     (501) staff       (20)     3297 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1307 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4470 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    12025 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1009 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     4464 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/optrepo.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1307 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5535 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/
+-rw-r--r--   0 runner     (501) staff       (20)     3507 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      716 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     1927 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     6138 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/MyModelTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12406 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)    10700 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2448 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     4172 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      205 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9847 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/simulation/simulator.py
+-rw-r--r--   0 runner     (501) staff       (20)    14960 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/utils/
+-rw-r--r--   0 runner     (501) staff       (20)    10317 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/utils/model_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      735 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/utils/logging.py
+-rw-r--r--   0 runner     (501) staff       (20)    10524 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/utils/compression.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/utils/context.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/
+-rwxr-xr-x   0 runner     (501) staff       (20)      313 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/cli_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)    17332 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    11014 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2263 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5644 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/docker_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    53261 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_runner.py
+-rw-r--r--   0 runner     (501) staff       (20)    19884 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)    10779 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_diagnosis.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2846 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/client_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3126 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/edge_deployment/simulator_daemon.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cli/model_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)     5828 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_inference.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2317 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_client_daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)     8771 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/modelops_configs.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_server_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    75936 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_server_runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    25678 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_cards.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_client_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5417 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/docker_client_login.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    16456 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_server_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    18262 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_cache.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    40997 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_deployment.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      816 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_server_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1766 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_object.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    26762 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_db.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6311 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_login_entry.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14992 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_client_data_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    22536 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_server_constants.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     8362 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_monitor.py
+-rw-r--r--   0 runner     (501) staff       (20)    29071 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_client_constants.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    47302 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_client_runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5442 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/docker_server_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2979 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_server_daemon.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6722 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_client_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2766 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_msg_object.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2906 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/model_deployment/device_model_inference_entry.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/env/
+-rw-r--r--   0 runner     (501) staff       (20)     3453 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/env/collect_env.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/env/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    45651 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/cli.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      629 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/torch_client.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      650 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cli/comm_utils/
+-rw-r--r--   0 runner     (501) staff       (20)    25892 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/comm_utils/sys_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/comm_utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      295 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/comm_utils/yaml_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cli/server_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)      749 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/server_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    71302 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/server_runner.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2848 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/job_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5677 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/docker_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1971 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/server_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    10533 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/app_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2519 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/server_daemon.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/cli/server_deployment/templates/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/templates/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/templates/fedml-aggregator-data-pv.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      279 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/templates/fedml-aggregator-data-pvc.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      275 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/templates/fedml-server-svc.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     1841 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)    13871 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/server_login.py
+-rw-r--r--   0 runner     (501) staff       (20)    18216 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cli/server_deployment/server_constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cheetah/
+-rw-r--r--   0 runner     (501) staff       (20)      153 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cheetah/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15566 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1939 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2047 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml/cheetah/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/cheetah/client/fedml_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/ml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/ml/aggregator/
+-rw-r--r--   0 runner     (501) staff       (20)      548 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/aggregator_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2488 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/default_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5621 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2408 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)    10546 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/agg_operator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3388 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/ml/engine/
+-rw-r--r--   0 runner     (501) staff       (20)    11333 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/engine/ml_engine_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/engine/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1345 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/engine/torch_process_group_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/ml/trainer/
+-rw-r--r--   0 runner     (501) staff       (20)     3953 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/scaffold_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      580 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/trainer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)     9496 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/fednova_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/local_optimizer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5923 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/fedprox_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3578 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     6857 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/feddyn_trainer copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     5180 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/feddyn_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5063 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     6274 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/mime_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4026 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer_tag_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)     5805 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/linear/
+-rw-r--r--   0 runner     (501) staff       (20)      433 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/linear/lr.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/linear/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      544 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/linear/lr_cifar10.py
+-rw-r--r--   0 runner     (501) staff       (20)       52 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4549 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/model_hub.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/mobile/
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/mobile/mnn_lenet.py
+-rw-r--r--   0 runner     (501) staff       (20)     3860 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/mobile/mnn_resnet.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/mobile/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      774 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/mobile/torch_lenet.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/nlp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/nlp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6272 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/nlp/model_args.py
+-rw-r--r--   0 runner     (501) staff       (20)     4687 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/nlp/rnn.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/finance/
+-rw-r--r--   0 runner     (501) staff       (20)      458 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/finance/vfl_feature_extractor.py
+-rw-r--r--   0 runner     (501) staff       (20)     2385 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/finance/vfl_models_standalone.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/finance/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      354 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/finance/vfl_classifier.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/cv/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/cv/resnet56/
+-rw-r--r--   0 runner     (501) staff       (20)     9541 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet56/resnet_pretrained.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet56/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8241 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet56/resnet_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     9507 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet56/resnet_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     6216 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/vgg.py
+-rw-r--r--   0 runner     (501) staff       (20)      455 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/test_cnn.py
+-rw-r--r--   0 runner     (501) staff       (20)    16186 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet_torch.py
+-rw-r--r--   0 runner     (501) staff       (20)    25891 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/efficientnet_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7751 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10352 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/mobilenet_v3.py
+-rw-r--r--   0 runner     (501) staff       (20)    19954 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/batchnorm_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7629 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/cnn.py
+-rw-r--r--   0 runner     (501) staff       (20)     1590 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/mnist_gan.py
+-rw-r--r--   0 runner     (501) staff       (20)    17984 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/efficientnet.py
+-rw-r--r--   0 runner     (501) staff       (20)    25096 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet_all.py
+-rw-r--r--   0 runner     (501) staff       (20)     4593 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/mobilenet.py
+-rw-r--r--   0 runner     (501) staff       (20)    74592 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/common.py
+-rw-r--r--   0 runner     (501) staff       (20)    10274 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/model/cv/darts/
+-rw-r--r--   0 runner     (501) staff       (20)     7088 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/model_search_gdas.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1713 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/visualize.py
+-rw-r--r--   0 runner     (501) staff       (20)    18693 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/architect.py
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     4504 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/operations.py
+-rw-r--r--   0 runner     (501) staff       (20)     3268 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    12302 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/model_search.py
+-rw-r--r--   0 runner     (501) staff       (20)     8673 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/train.py
+-rw-r--r--   0 runner     (501) staff       (20)     3486 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/genotypes.py
+-rw-r--r--   0 runner     (501) staff       (20)    14555 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/darts/train_search.py
+-rw-r--r--   0 runner     (501) staff       (20)     7625 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/resnet_gn.py
+-rw-r--r--   0 runner     (501) staff       (20)     5343 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/model/cv/group_normalization.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/device/
+-rw-r--r--   0 runner     (501) staff       (20)     2833 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/device/gpu_mapping_cross_silo.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/device/gpu_mapping_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)     5611 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/device/device.py
+-rw-r--r--   0 runner     (501) staff       (20)      112 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/device/ip_config_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/runner.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/cross_silo/
+-rw-r--r--   0 runner     (501) staff       (20)      673 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/fa_server.py
+-rw-r--r--   0 runner     (501) staff       (20)      644 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/fa_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      186 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/cross_silo/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2224 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11189 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     5262 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      879 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/server/server_initializer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/
+-rw-r--r--   0 runner     (501) staff       (20)     1526 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2714 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/message_define.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2051 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/fa_local_analyzer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2050 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6118 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/cross_silo/client/fedml_client_master_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/aggregator/
+-rw-r--r--   0 runner     (501) staff       (20)     1903 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/frequency_estimation_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1885 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/intersection_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1559 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/union_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/avg_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3908 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/k_percentile_element_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4005 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/heavy_hitter_triehh_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/aggregator/global_analyzer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      414 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/simulation/sp/
+-rw-r--r--   0 runner     (501) staff       (20)     1192 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/simulation/sp/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/simulation/sp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3449 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/simulation/sp/simulator.py
+-rw-r--r--   0 runner     (501) staff       (20)      119 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/simulation/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      606 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/simulation/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2832 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/utils/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7789 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/utils/trie.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/
+-rw-r--r--   0 runner     (501) staff       (20)     1599 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/heavy_hitter_triehh.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      453 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/frequency_estimation.py
+-rw-r--r--   0 runner     (501) staff       (20)     1413 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/client_analyzer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      392 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/k_percentage_element.py
+-rw-r--r--   0 runner     (501) staff       (20)      223 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/intersection.py
+-rw-r--r--   0 runner     (501) staff       (20)      217 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/union.py
+-rw-r--r--   0 runner     (501) staff       (20)      362 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/local_analyzer/avg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/base_frame/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/base_frame/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      716 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/base_frame/server_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1049 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/base_frame/client_analyzer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/data/
+-rw-r--r--   0 runner     (501) staff       (20)     4487 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/data_loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/data/twitter_Sentiment140/
+-rw-r--r--   0 runner     (501) staff       (20)     3223 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py
+-rw-r--r--   0 runner     (501) staff       (20)     1693 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/twitter_Sentiment140/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/twitter_Sentiment140/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       75 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2374 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/data/self_defined_data/
+-rw-r--r--   0 runner     (501) staff       (20)      856 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/self_defined_data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/self_defined_data/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/fa/data/fake_numeric_data/
+-rw-r--r--   0 runner     (501) staff       (20)      526 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/fake_numeric_data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/fa/data/fake_numeric_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      545 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/launch_cross_device.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/MNIST/
+-rw-r--r--   0 runner     (501) staff       (20)     5448 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/MNIST/mnist_mobile_preprocessor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4945 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/MNIST/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/MNIST/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/MNIST/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/lending_club_loan/
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/lending_club_loan/lending_club_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/lending_club_loan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2291 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/lending_club_loan/lending_club_feature_group.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fed_cifar100/
+-rw-r--r--   0 runner     (501) staff       (20)     6320 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_cifar100/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_cifar100/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      517 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_cifar100/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2631 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_cifar100/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/FederatedEMNIST/
+-rw-r--r--   0 runner     (501) staff       (20)     6737 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/FederatedEMNIST/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/FederatedEMNIST/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      426 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/FederatedEMNIST/dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/cifar100/
+-rw-r--r--   0 runner     (501) staff       (20)    11837 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar100/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2077 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar100/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar100/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    21968 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)      156 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/file_operation.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/shakespeare/
+-rwxr-xr-x   0 runner     (501) staff       (20)     3431 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/shakespeare/language_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4135 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/shakespeare/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/shakespeare/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      335 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/shakespeare/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/shakespeare/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/synthetic_1_1/
+-rw-r--r--   0 runner     (501) staff       (20)     4562 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/synthetic_1_1/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/synthetic_1_1/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3210 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/synthetic_1_1/stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     2749 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/synthetic_1_1/generate_synthetic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/Landmarks/
+-rw-r--r--   0 runner     (501) staff       (20)      375 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/download_with_tff.py
+-rw-r--r--   0 runner     (501) staff       (20)    14871 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/download_without_tff.py
+-rw-r--r--   0 runner     (501) staff       (20)    11159 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2191 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14342 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2090 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/check_download.py
+-rw-r--r--   0 runner     (501) staff       (20)     7872 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/Landmarks/download_without_tf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fednlp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fednlp/base/
+-rw-r--r--   0 runner     (501) staff       (20)      169 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/globals.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fednlp/base/preprocess/
+-rw-r--r--   0 runner     (501) staff       (20)     4794 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/preprocess/base_example.py
+-rw-r--r--   0 runner     (501) staff       (20)      363 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/preprocess/base_data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/preprocess/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      224 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/preprocess/base_preprocessor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fednlp/base/raw_data/
+-rw-r--r--   0 runner     (501) staff       (20)     1428 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/raw_data/partition.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/raw_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fednlp/base/data_manager/
+-rw-r--r--   0 runner     (501) staff       (20)    16505 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/data_manager/base_data_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/data_manager/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8248 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fednlp/base/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/NUS_WIDE/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/NUS_WIDE/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11281 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/NUS_WIDE/nus_wide_dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/stackoverflow_lr/
+-rw-r--r--   0 runner     (501) staff       (20)     8487 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_lr/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_lr/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2841 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_lr/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     4272 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_lr/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/fed_shakespeare/
+-rw-r--r--   0 runner     (501) staff       (20)     6100 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_shakespeare/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_shakespeare/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/fed_shakespeare/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/ImageNet/
+-rw-r--r--   0 runner     (501) staff       (20)    11416 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/ImageNet/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     6718 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/ImageNet/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/ImageNet/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5874 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/ImageNet/datasets_hdf5.py
+-rw-r--r--   0 runner     (501) staff       (20)     1429 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/data_loader_cross_silo.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/cinic10/
+-rw-r--r--   0 runner     (501) staff       (20)    13807 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cinic10/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     3071 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cinic10/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cinic10/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/stackoverflow_nwp/
+-rw-r--r--   0 runner     (501) staff       (20)     7023 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_nwp/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_nwp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2171 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_nwp/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2508 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/stackoverflow_nwp/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/UCI/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/UCI/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6215 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/UCI/data_loader_for_susy_and_ro.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/edge_case_examples/
+-rw-r--r--   0 runner     (501) staff       (20)    44697 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/edge_case_examples/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)    20285 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/edge_case_examples/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/edge_case_examples/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:20.000000 fedml-0.8.7a4/fedml/data/cifar10/
+-rw-r--r--   0 runner     (501) staff       (20)    13696 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar10/efficient_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)    11902 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar10/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2378 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar10/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)     3972 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar10/without_reload.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-14 19:14:07.000000 fedml-0.8.7a4/fedml/data/cifar10/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3806 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    48148 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)       45 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      546 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       21 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-14 19:14:19.000000 fedml-0.8.7a4/fedml.egg-info/dependency_links.txt
```

### Comparing `fedml-0.8.7a3/PKG-INFO` & `fedml-0.8.7a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml
-Version: 0.8.7a3
+Version: 0.8.7a4
 Summary: A research and production integrated edge-cloud library for federated/distributed machine learning at anywhere at any scale.
 Home-page: https://github.com/FedML-AI/FedML
 Author: FedML Team
 Author-email: ch@fedml.ai
 License: Apache 2.0
 Description: # FedML - The community building and connecting AI anywhere at any scale
```

### Comparing `fedml-0.8.7a3/tests/security/attack/test_label_flipping_attack.py` & `fedml-0.8.7a4/tests/security/attack/test_label_flipping_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/test_backdoor.py` & `fedml-0.8.7a4/tests/security/attack/test_backdoor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/test_model_replacement_backdoor_attack.py` & `fedml-0.8.7a4/tests/security/attack/test_model_replacement_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/test_invertgradient.py` & `fedml-0.8.7a4/tests/security/attack/test_invertgradient.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/test_byzantine_attack.py` & `fedml-0.8.7a4/tests/security/attack/test_byzantine_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/utils.py` & `fedml-0.8.7a4/tests/security/attack/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/test_edge_case_backdoor_attack.py` & `fedml-0.8.7a4/tests/security/attack/test_edge_case_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/attack/test_dlg.py` & `fedml-0.8.7a4/tests/security/attack/test_dlg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_residual_based_reweighting.py` & `fedml-0.8.7a4/tests/security/defense/test_residual_based_reweighting.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_wbc.py` & `fedml-0.8.7a4/tests/security/defense/test_wbc.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_crfl.py` & `fedml-0.8.7a4/tests/security/defense/test_crfl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_geometric_median.py` & `fedml-0.8.7a4/tests/security/defense/test_geometric_median.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_slsgd_defense.py` & `fedml-0.8.7a4/tests/security/defense/test_slsgd_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_weak_dp.py` & `fedml-0.8.7a4/tests/security/defense/test_weak_dp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_norm_diff_clipping.py` & `fedml-0.8.7a4/tests/security/defense/test_norm_diff_clipping.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/utils.py` & `fedml-0.8.7a4/tests/security/defense/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_bulyan.py` & `fedml-0.8.7a4/tests/security/defense/test_bulyan.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_robust_learning_rate_defense.py` & `fedml-0.8.7a4/tests/security/defense/test_robust_learning_rate_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_coordinate_wise_trimmed_mean.py` & `fedml-0.8.7a4/tests/security/defense/test_coordinate_wise_trimmed_mean.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_krum.py` & `fedml-0.8.7a4/tests/security/defense/test_krum.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_cclip.py` & `fedml-0.8.7a4/tests/security/defense/test_cclip.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_foolsgold_defense.py` & `fedml-0.8.7a4/tests/security/defense/test_foolsgold_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/tests/security/defense/test_soteria.py` & `fedml-0.8.7a4/tests/security/defense/test_soteria.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/README.md` & `fedml-0.8.7a4/README.md`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/setup.py` & `fedml-0.8.7a4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 
 # if platform.machine() == "x86_64":
 #    requirements.append("MNN==1.1.6")
 
 setup(
     name="fedml",
-    version="0.8.7a3",
+    version="0.8.7a4",
     author="FedML Team",
     author_email="ch@fedml.ai",
     description="A research and production integrated edge-cloud library for "
                 "federated/distributed machine learning at anywhere at any scale.",
     long_description=io.open(os.path.join("README.md"), "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/FedML-AI/FedML",
```

### Comparing `fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.7a4/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py` & `fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py` & `fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py` & `fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py` & `fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py` & `fedml-0.8.7a4/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py` & `fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py` & `fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py` & `fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py` & `fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py` & `fedml-0.8.7a4/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.7a4/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py` & `fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py` & `fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py` & `fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py` & `fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py` & `fedml-0.8.7a4/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py` & `fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py` & `fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py` & `fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py` & `fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py` & `fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py` & `fedml-0.8.7a4/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py` & `fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py` & `fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py` & `fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py` & `fedml-0.8.7a4/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/centralized/main.py` & `fedml-0.8.7a4/examples/centralized/main.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/reddit_trainer.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/reddit_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg/main.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg/main.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.7a4/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/launch_serving.py` & `fedml-0.8.7a4/fedml/launch_serving.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/launch_cross_silo_hi.py` & `fedml-0.8.7a4/fedml/launch_cross_silo_hi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/runner.py` & `fedml-0.8.7a4/fedml/runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_message_define.py` & `fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py` & `fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py` & `fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py` & `fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/lightsecagg/lsa_fedml_api.py` & `fedml-0.8.7a4/fedml/cross_silo/lightsecagg/lsa_fedml_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/server/message_define.py` & `fedml-0.8.7a4/fedml/cross_silo/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/server/fedml_server_manager.py` & `fedml-0.8.7a4/fedml/cross_silo/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/server/fedml_aggregator.py` & `fedml-0.8.7a4/fedml/cross_silo/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/server/server_initializer.py` & `fedml-0.8.7a4/fedml/cross_silo/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/fedml_client.py` & `fedml-0.8.7a4/fedml/cross_silo/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/fedml_server.py` & `fedml-0.8.7a4/fedml/cross_silo/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/client_initializer.py` & `fedml-0.8.7a4/fedml/cross_silo/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/client_launcher.py` & `fedml-0.8.7a4/fedml/cross_silo/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/message_define.py` & `fedml-0.8.7a4/fedml/cross_silo/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.7a4/fedml/cross_silo/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/fedml_client_slave_manager.py` & `fedml-0.8.7a4/fedml/cross_silo/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/process_group_manager.py` & `fedml-0.8.7a4/fedml/cross_silo/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/utils.py` & `fedml-0.8.7a4/fedml/cross_silo/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/fedml_client_master_manager.py` & `fedml-0.8.7a4/fedml/cross_silo/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_silo/client/fedml_trainer.py` & `fedml-0.8.7a4/fedml/cross_silo/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/launch_cross_silo_horizontal.py` & `fedml-0.8.7a4/fedml/launch_cross_silo_horizontal.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/server/message_define.py` & `fedml-0.8.7a4/fedml/serving/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/server/fedml_server_manager.py` & `fedml-0.8.7a4/fedml/serving/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/server/fedml_aggregator.py` & `fedml-0.8.7a4/fedml/serving/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/server/server_initializer.py` & `fedml-0.8.7a4/fedml/serving/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/fedml_client.py` & `fedml-0.8.7a4/fedml/serving/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/fedml_server.py` & `fedml-0.8.7a4/fedml/serving/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/client_initializer.py` & `fedml-0.8.7a4/fedml/serving/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/client_launcher.py` & `fedml-0.8.7a4/fedml/serving/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/message_define.py` & `fedml-0.8.7a4/fedml/serving/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.7a4/fedml/serving/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/fedml_client_slave_manager.py` & `fedml-0.8.7a4/fedml/serving/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/process_group_manager.py` & `fedml-0.8.7a4/fedml/serving/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/utils.py` & `fedml-0.8.7a4/fedml/serving/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/fedml_client_master_manager.py` & `fedml-0.8.7a4/fedml/serving/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/serving/client/fedml_trainer.py` & `fedml-0.8.7a4/fedml/serving/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/schedule/runtime_estimate.py` & `fedml-0.8.7a4/fedml/core/schedule/runtime_estimate.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/schedule/seq_train_scheduler.py` & `fedml-0.8.7a4/fedml/core/schedule/seq_train_scheduler.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/alg_frame/params.py` & `fedml-0.8.7a4/fedml/core/alg_frame/params.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/alg_frame/client_trainer.py` & `fedml-0.8.7a4/fedml/core/alg_frame/client_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/alg_frame/context.py` & `fedml-0.8.7a4/fedml/core/alg_frame/context.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/alg_frame/server_aggregator.py` & `fedml-0.8.7a4/fedml/core/alg_frame/server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/topology/asymmetric_topology_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/topology/asymmetric_topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/topology/symmetric_topology_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/topology/symmetric_topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/crypto/crypto_api.py` & `fedml-0.8.7a4/fedml/core/distributed/crypto/crypto_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/fedml_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/fedml_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/s3/remote_storage_mnn.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/s3/remote_storage_mnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/s3/remote_storage.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/s3/remote_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/s3/utils.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/s3/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mpi/mpi_send_thread.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mpi/mpi_send_thread.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mpi/com_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mpi/com_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mpi/mpi_receive_thread.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mpi/mpi_receive_thread.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_server.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/trpc/trpc_server.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/trpc/trpc_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/trpc/trpc_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/trpc/trpc_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/message.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/message.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/utils.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/base_com_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/base_com_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mqtt/mqtt_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mqtt/mqtt_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py` & `fedml-0.8.7a4/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py` & `fedml-0.8.7a4/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py` & `fedml-0.8.7a4/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/flow/fedml_flow.py` & `fedml-0.8.7a4/fedml/core/distributed/flow/fedml_flow.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/flow/fedml_executor.py` & `fedml-0.8.7a4/fedml/core/distributed/flow/fedml_executor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/distributed/flow/test_fedml_flow.py` & `fedml-0.8.7a4/fedml/core/distributed/flow/test_fedml_flow.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/model_replacement_backdoor_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/model_replacement_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/attack_base.py` & `fedml-0.8.7a4/fedml/core/security/attack/attack_base.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/edge_case_backdoor_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/edge_case_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/byzantine_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/byzantine_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/lazy_worker.py` & `fedml-0.8.7a4/fedml/core/security/attack/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/invert_gradient_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/invert_gradient_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/dlg_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/dlg_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/revealing_labels_from_gradients_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/revealing_labels_from_gradients_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/label_flipping_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/label_flipping_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/attack/backdoor_attack.py` & `fedml-0.8.7a4/fedml/core/security/attack/backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/fedml_attacker.py` & `fedml-0.8.7a4/fedml/core/security/fedml_attacker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/constants.py` & `fedml-0.8.7a4/fedml/core/security/constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/fedml_defender.py` & `fedml-0.8.7a4/fedml/core/security/fedml_defender.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/common/bucket.py` & `fedml-0.8.7a4/fedml/core/security/common/bucket.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/common/net.py` & `fedml-0.8.7a4/fedml/core/security/common/net.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/common/attack_defense_data_loader.py` & `fedml-0.8.7a4/fedml/core/security/common/attack_defense_data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/common/utils.py` & `fedml-0.8.7a4/fedml/core/security/common/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/three_sigma_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/three_sigma_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/norm_diff_clipping_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/norm_diff_clipping_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/residual_based_reweighting_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/residual_based_reweighting_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/three_sigma_krum_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/three_sigma_krum_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/slsgd_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/slsgd_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/coordinate_wise_median_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/coordinate_wise_median_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/wbc_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/wbc_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/robust_learning_rate_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/robust_learning_rate_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/RFA_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/RFA_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/defense_base.py` & `fedml-0.8.7a4/fedml/core/security/defense/defense_base.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/foolsgold_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/foolsgold_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/soteria_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/soteria_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/bulyan_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/bulyan_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/cross_round_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/cross_round_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/three_sigma_geomedian_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/three_sigma_geomedian_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/geometric_median_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/geometric_median_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/crfl_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/crfl_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/outlier_detection.py` & `fedml-0.8.7a4/fedml/core/security/defense/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/weak_dp_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/weak_dp_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/cclip_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/cclip_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/security/defense/krum_defense.py` & `fedml-0.8.7a4/fedml/core/security/defense/krum_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_configs.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_configs.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt` & `fedml-0.8.7a4/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt` & `fedml-0.8.7a4/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/ssl/open-root-ca.crt` & `fedml-0.8.7a4/fedml/core/mlops/ssl/open-root-ca.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt` & `fedml-0.8.7a4/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_metrics.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_metrics.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_profiler_event.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_profiler_event.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_status.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_status.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/__init__.py` & `fedml-0.8.7a4/fedml/core/mlops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/stats_impl.py` & `fedml-0.8.7a4/fedml/core/mlops/stats_impl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_utils.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_runtime_log_daemon.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_runtime_log_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/system_stats.py` & `fedml-0.8.7a4/fedml/core/mlops/system_stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mlops/mlops_runtime_log.py` & `fedml-0.8.7a4/fedml/core/mlops/mlops_runtime_log.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/__init__.py` & `fedml-0.8.7a4/fedml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mpc/lightsecagg.py` & `fedml-0.8.7a4/fedml/core/mpc/lightsecagg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/mpc/secagg.py` & `fedml-0.8.7a4/fedml/core/mpc/secagg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/mechanisms/dp_mechanism.py` & `fedml-0.8.7a4/fedml/core/dp/mechanisms/dp_mechanism.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/mechanisms/laplace.py` & `fedml-0.8.7a4/fedml/core/dp/mechanisms/laplace.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/mechanisms/gaussian.py` & `fedml-0.8.7a4/fedml/core/dp/mechanisms/gaussian.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/test/test_fed_privacy_mechanism.py` & `fedml-0.8.7a4/fedml/core/dp/test/test_fed_privacy_mechanism.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/fedml_differential_privacy.py` & `fedml-0.8.7a4/fedml/core/dp/fedml_differential_privacy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/frames/NbAFL.py` & `fedml-0.8.7a4/fedml/core/dp/frames/NbAFL.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/frames/dp_clip.py` & `fedml-0.8.7a4/fedml/core/dp/frames/dp_clip.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/frames/cdp.py` & `fedml-0.8.7a4/fedml/core/dp/frames/cdp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/frames/base_dp_solution.py` & `fedml-0.8.7a4/fedml/core/dp/frames/base_dp_solution.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/budget_accountant/rdp_analysis.py` & `fedml-0.8.7a4/fedml/core/dp/budget_accountant/rdp_analysis.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/budget_accountant/__init__.py` & `fedml-0.8.7a4/fedml/core/dp/budget_accountant/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/budget_accountant/rdp_accountant.py` & `fedml-0.8.7a4/fedml/core/dp/budget_accountant/rdp_accountant.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/dp/common/utils.py` & `fedml-0.8.7a4/fedml/core/dp/common/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/contribution/gtg_shapley_value.py` & `fedml-0.8.7a4/fedml/core/contribution/gtg_shapley_value.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/contribution/mr_shapley_value.py` & `fedml-0.8.7a4/fedml/core/contribution/mr_shapley_value.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/contribution/base_contribution_assessor.py` & `fedml-0.8.7a4/fedml/core/contribution/base_contribution_assessor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/contribution/leave_one_out.py` & `fedml-0.8.7a4/fedml/core/contribution/leave_one_out.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/contribution/contribution_assessor_manager.py` & `fedml-0.8.7a4/fedml/core/contribution/contribution_assessor_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/core/data/noniid_partition.py` & `fedml-0.8.7a4/fedml/core/data/noniid_partition.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/config/simulaton_mpi/fedml_config.yaml` & `fedml-0.8.7a4/fedml/config/simulaton_mpi/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/config/simulation_sp/fedml_config.yaml` & `fedml-0.8.7a4/fedml/config/simulation_sp/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/arguments.py` & `fedml-0.8.7a4/fedml/arguments.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/mlops/__init__.py` & `fedml-0.8.7a4/fedml/mlops/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/launch_cheeath.py` & `fedml-0.8.7a4/fedml/launch_cheeath.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/constants.py` & `fedml-0.8.7a4/fedml/constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_device/server_mnn/message_define.py` & `fedml-0.8.7a4/fedml/cross_device/server_mnn/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_device/server_mnn/fedml_server_manager.py` & `fedml-0.8.7a4/fedml/cross_device/server_mnn/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_device/server_mnn/utils.py` & `fedml-0.8.7a4/fedml/cross_device/server_mnn/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_device/server_mnn/fedml_aggregator.py` & `fedml-0.8.7a4/fedml/cross_device/server_mnn/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_device/server_mnn/server_mnn_api.py` & `fedml-0.8.7a4/fedml/cross_device/server_mnn/server_mnn_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cross_device/mnn_server.py` & `fedml-0.8.7a4/fedml/cross_device/mnn_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/centralized/centralized_trainer.py` & `fedml-0.8.7a4/fedml/centralized/centralized_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/launch_simulation.py` & `fedml-0.8.7a4/fedml/launch_simulation.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedavg/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedavg/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedavg/fedavg_api.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedavg/fedavg_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedprox/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedprox/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedprox/fedprox_trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedprox/fedprox_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/TA_trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/TA_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/mpc_function.py` & `fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/mpc_function.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/turboaggregate/TA_client.py` & `fedml-0.8.7a4/fedml/simulation/sp/turboaggregate/TA_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/feddyn/client copy.py` & `fedml-0.8.7a4/fedml/simulation/sp/feddyn/client copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/feddyn/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/feddyn/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/feddyn/feddyn_trainer copy.py` & `fedml-0.8.7a4/fedml/simulation/sp/feddyn/feddyn_trainer copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/feddyn/feddyn_trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/feddyn/feddyn_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/party_models.py` & `fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/party_models.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/vfl.py` & `fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/vfl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/vfl_api.py` & `fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/vfl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py` & `fedml-0.8.7a4/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fednova/fednova.py` & `fedml-0.8.7a4/fedml/simulation/sp/fednova/fednova.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fednova/fednova_trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/fednova/fednova_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fednova/fednova_api.py` & `fedml-0.8.7a4/fedml/simulation/sp/fednova/fednova_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fednova/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/fednova/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fednova/comm_helpers.py` & `fedml-0.8.7a4/fedml/simulation/sp/fednova/comm_helpers.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedopt/fedopt_api.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedopt/fedopt_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedopt/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedopt/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/fedopt/optrepo.py` & `fedml-0.8.7a4/fedml/simulation/sp/fedopt/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/group.py` & `fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/group.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/hierarchical_fl/trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/hierarchical_fl/trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/mime/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/mime/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/mime/opt_utils.py` & `fedml-0.8.7a4/fedml/simulation/sp/mime/opt_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/mime/mime_trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/mime/mime_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/scaffold/scaffold_trainer.py` & `fedml-0.8.7a4/fedml/simulation/sp/scaffold/scaffold_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/scaffold/client.py` & `fedml-0.8.7a4/fedml/simulation/sp/scaffold/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/decentralized/decentralized_fl_api.py` & `fedml-0.8.7a4/fedml/simulation/sp/decentralized/decentralized_fl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/decentralized/client_dsgd.py` & `fedml-0.8.7a4/fedml/simulation/sp/decentralized/client_dsgd.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/decentralized/client_pushsum.py` & `fedml-0.8.7a4/fedml/simulation/sp/decentralized/client_pushsum.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/sp/decentralized/topology_manager.py` & `fedml-0.8.7a4/fedml/simulation/sp/decentralized/topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAvgClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAVGAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAvgAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAvgAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAVGTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg/FedAvgServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg/FedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/split_nn/server.py` & `fedml-0.8.7a4/fedml/simulation/mpi/split_nn/server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/split_nn/SplitNNAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/split_nn/SplitNNAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/split_nn/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/split_nn/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/split_nn/client.py` & `fedml-0.8.7a4/fedml/simulation/mpi/split_nn/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/split_nn/client_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/split_nn/client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/split_nn/server_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/split_nn/server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedprox/FedProxAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedprox/FedProxAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGanServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGanServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGanAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGanAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/gan_trainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/gan_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGANTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGANTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGANAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGANAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgan/FedGanClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgan/FedGanClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/FedGKTAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/FedGKTAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/message_def.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/message_def.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/base_framework/client_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/base_framework/client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/base_framework/central_worker.py` & `fedml-0.8.7a4/fedml/simulation/mpi/base_framework/central_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/base_framework/algorithm_api.py` & `fedml-0.8.7a4/fedml/simulation/mpi/base_framework/algorithm_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/base_framework/central_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/base_framework/central_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py` & `fedml-0.8.7a4/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py` & `fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/decentralized_framework/algorithm_api.py` & `fedml-0.8.7a4/fedml/simulation/mpi/decentralized_framework/algorithm_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py` & `fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/classical_vertical_fl/host_manager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/classical_vertical_fl/host_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednas/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednas/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednas/FedNASServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednas/FedNASServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/FedNovaAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/FedNovaAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fednova/my_model_trainer_classification.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fednova/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/optrepo.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt/FedOptServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt/FedOptServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/optrepo.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegClientManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/message_define.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/MyModelTrainer.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/MyModelTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegAggregator.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/utils.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegAPI.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/mpi/fedseg/FedSegServerManager.py` & `fedml-0.8.7a4/fedml/simulation/mpi/fedseg/FedSegServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/simulation/simulator.py` & `fedml-0.8.7a4/fedml/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/__init__.py` & `fedml-0.8.7a4/fedml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     FEDML_TRAINING_PLATFORM_SERVING,
 )
 from .core.common.ml_engine_backend import MLEngineBackend
 
 _global_training_type = None
 _global_comm_backend = None
 
-__version__ = "0.8.7a3"
+__version__ = "0.8.7a4"
 
 
 def init(args=None):
     if args is None:
         args = load_arguments(fedml._global_training_type, fedml._global_comm_backend)
 
     """Initialize FedML Engine."""
```

### Comparing `fedml-0.8.7a3/fedml/utils/model_utils.py` & `fedml-0.8.7a4/fedml/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/utils/logging.py` & `fedml-0.8.7a4/fedml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/utils/compression.py` & `fedml-0.8.7a4/fedml/utils/compression.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/utils/context.py` & `fedml-0.8.7a4/fedml/utils/context.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_data_interface.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_login.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_daemon.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/docker_login.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/docker_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_runner.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_constants.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_diagnosis.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_diagnosis.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/client_api.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/client_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/edge_deployment/simulator_daemon.py` & `fedml-0.8.7a4/fedml/cli/edge_deployment/simulator_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_inference.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_inference.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_client_daemon.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_client_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/modelops_configs.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/modelops_configs.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_server_api.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_server_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_server_runner.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_server_runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_cards.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_cards.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_client_api.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_client_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/docker_client_login.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/docker_client_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_server_login.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_server_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_cache.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_cache.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_deployment.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_deployment.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_server_data_interface.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_server_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_object.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_object.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_db.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_db.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_login_entry.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_login_entry.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_client_data_interface.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_client_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_server_constants.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_server_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_monitor.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_monitor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_client_constants.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_client_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_client_runner.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_client_runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/docker_server_login.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/docker_server_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_server_daemon.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_server_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_client_login.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_client_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_msg_object.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_msg_object.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/model_deployment/device_model_inference_entry.py` & `fedml-0.8.7a4/fedml/cli/model_deployment/device_model_inference_entry.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/env/collect_env.py` & `fedml-0.8.7a4/fedml/cli/env/collect_env.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/cli.py` & `fedml-0.8.7a4/fedml/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml` & `fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml` & `fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml` & `fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml` & `fedml-0.8.7a4/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/comm_utils/sys_utils.py` & `fedml-0.8.7a4/fedml/cli/comm_utils/sys_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -564,26 +564,34 @@
 
 def run_cmd(command, show_local_console=False):
     process = ClientConstants.exec_console_with_script(command, should_capture_stdout=True,
                                                        should_capture_stderr=True)
     ret_code, out, err = ClientConstants.get_console_pipe_out_err_results(process)
     if ret_code is None or ret_code <= 0:
         if out is not None:
-            out_str = out.decode(encoding="utf-8")
+            try:
+                out_str = out.decode(encoding="utf-8")
+            except:
+                logging.info("utf-8 could not decode the output msg")
+                out_str = ""
             if out_str != "":
                 logging.info("{}".format(out_str))
                 if show_local_console:
                     print(out_str)
 
         log_return_info(command, 0)
 
         is_cmd_run_ok = True
     else:
         if err is not None:
-            err_str = err.decode(encoding="utf-8")
+            try:
+                err_str = err.decode(encoding="utf-8")
+            except:
+                logging.info("utf-8 could not decode the err msg")
+                err_str = ""
             if err_str != "":
                 logging.error("{}".format(err_str))
                 if show_local_console:
                     print(err_str)
 
         log_return_info(command, ret_code)
```

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/server_data_interface.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/server_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/server_runner.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/server_runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/job_manager.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/job_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/docker_login.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/docker_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/server_api.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/server_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/app_manager.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/app_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/server_daemon.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/server_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml` & `fedml-0.8.7a4/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/server_login.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/server_login.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cli/server_deployment/server_constants.py` & `fedml-0.8.7a4/fedml/cli/server_deployment/server_constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/server/message_define.py` & `fedml-0.8.7a4/fedml/cheetah/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/server/fedml_server_manager.py` & `fedml-0.8.7a4/fedml/cheetah/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/server/fedml_aggregator.py` & `fedml-0.8.7a4/fedml/cheetah/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/server/server_initializer.py` & `fedml-0.8.7a4/fedml/cheetah/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/fedml_client.py` & `fedml-0.8.7a4/fedml/cheetah/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/fedml_server.py` & `fedml-0.8.7a4/fedml/cheetah/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/client_initializer.py` & `fedml-0.8.7a4/fedml/cheetah/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/client_launcher.py` & `fedml-0.8.7a4/fedml/cheetah/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/message_define.py` & `fedml-0.8.7a4/fedml/cheetah/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.7a4/fedml/cheetah/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/fedml_client_slave_manager.py` & `fedml-0.8.7a4/fedml/cheetah/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/process_group_manager.py` & `fedml-0.8.7a4/fedml/cheetah/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/utils.py` & `fedml-0.8.7a4/fedml/cheetah/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/fedml_client_master_manager.py` & `fedml-0.8.7a4/fedml/cheetah/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/cheetah/client/fedml_trainer.py` & `fedml-0.8.7a4/fedml/cheetah/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/aggregator_creator.py` & `fedml-0.8.7a4/fedml/ml/aggregator/aggregator_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator_nwp.py` & `fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/default_aggregator.py` & `fedml-0.8.7a4/fedml/ml/aggregator/default_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator.py` & `fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator_classification.py` & `fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/agg_operator.py` & `fedml-0.8.7a4/fedml/ml/aggregator/agg_operator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/aggregator/my_server_aggregator_prediction.py` & `fedml-0.8.7a4/fedml/ml/aggregator/my_server_aggregator_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/engine/ml_engine_adapter.py` & `fedml-0.8.7a4/fedml/ml/engine/ml_engine_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/engine/torch_process_group_manager.py` & `fedml-0.8.7a4/fedml/ml/engine/torch_process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/scaffold_trainer.py` & `fedml-0.8.7a4/fedml/ml/trainer/scaffold_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/trainer_creator.py` & `fedml-0.8.7a4/fedml/ml/trainer/trainer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/fednova_trainer.py` & `fedml-0.8.7a4/fedml/ml/trainer/fednova_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/fedprox_trainer.py` & `fedml-0.8.7a4/fedml/ml/trainer/fedprox_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer_nwp.py` & `fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/feddyn_trainer copy.py` & `fedml-0.8.7a4/fedml/ml/trainer/feddyn_trainer copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/feddyn_trainer.py` & `fedml-0.8.7a4/fedml/ml/trainer/feddyn_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer.py` & `fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/mime_trainer.py` & `fedml-0.8.7a4/fedml/ml/trainer/mime_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer_tag_prediction.py` & `fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer_tag_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/ml/trainer/my_model_trainer_classification.py` & `fedml-0.8.7a4/fedml/ml/trainer/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/linear/lr_cifar10.py` & `fedml-0.8.7a4/fedml/model/linear/lr_cifar10.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/model_hub.py` & `fedml-0.8.7a4/fedml/model/model_hub.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/mobile/mnn_lenet.py` & `fedml-0.8.7a4/fedml/model/mobile/mnn_lenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/mobile/mnn_resnet.py` & `fedml-0.8.7a4/fedml/model/mobile/mnn_resnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/mobile/torch_lenet.py` & `fedml-0.8.7a4/fedml/model/mobile/torch_lenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/nlp/model_args.py` & `fedml-0.8.7a4/fedml/model/nlp/model_args.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/nlp/rnn.py` & `fedml-0.8.7a4/fedml/model/nlp/rnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/finance/vfl_models_standalone.py` & `fedml-0.8.7a4/fedml/model/finance/vfl_models_standalone.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet56/resnet_pretrained.py` & `fedml-0.8.7a4/fedml/model/cv/resnet56/resnet_pretrained.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet56/resnet_server.py` & `fedml-0.8.7a4/fedml/model/cv/resnet56/resnet_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet56/resnet_client.py` & `fedml-0.8.7a4/fedml/model/cv/resnet56/resnet_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/vgg.py` & `fedml-0.8.7a4/fedml/model/cv/vgg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet_torch.py` & `fedml-0.8.7a4/fedml/model/cv/resnet_torch.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/efficientnet_utils.py` & `fedml-0.8.7a4/fedml/model/cv/efficientnet_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet_cifar.py` & `fedml-0.8.7a4/fedml/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/mobilenet_v3.py` & `fedml-0.8.7a4/fedml/model/cv/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/batchnorm_utils.py` & `fedml-0.8.7a4/fedml/model/cv/batchnorm_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/cnn.py` & `fedml-0.8.7a4/fedml/model/cv/cnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/mnist_gan.py` & `fedml-0.8.7a4/fedml/model/cv/mnist_gan.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/efficientnet.py` & `fedml-0.8.7a4/fedml/model/cv/efficientnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet_all.py` & `fedml-0.8.7a4/fedml/model/cv/resnet_all.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/mobilenet.py` & `fedml-0.8.7a4/fedml/model/cv/mobilenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/common.py` & `fedml-0.8.7a4/fedml/model/cv/common.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet.py` & `fedml-0.8.7a4/fedml/model/cv/resnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/model_search_gdas.py` & `fedml-0.8.7a4/fedml/model/cv/darts/model_search_gdas.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/visualize.py` & `fedml-0.8.7a4/fedml/model/cv/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/architect.py` & `fedml-0.8.7a4/fedml/model/cv/darts/architect.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/model.py` & `fedml-0.8.7a4/fedml/model/cv/darts/model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/operations.py` & `fedml-0.8.7a4/fedml/model/cv/darts/operations.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/utils.py` & `fedml-0.8.7a4/fedml/model/cv/darts/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/model_search.py` & `fedml-0.8.7a4/fedml/model/cv/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/train.py` & `fedml-0.8.7a4/fedml/model/cv/darts/train.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/genotypes.py` & `fedml-0.8.7a4/fedml/model/cv/darts/genotypes.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/darts/train_search.py` & `fedml-0.8.7a4/fedml/model/cv/darts/train_search.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/resnet_gn.py` & `fedml-0.8.7a4/fedml/model/cv/resnet_gn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/model/cv/group_normalization.py` & `fedml-0.8.7a4/fedml/model/cv/group_normalization.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/device/gpu_mapping_cross_silo.py` & `fedml-0.8.7a4/fedml/device/gpu_mapping_cross_silo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/device/gpu_mapping_mpi.py` & `fedml-0.8.7a4/fedml/device/gpu_mapping_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/device/device.py` & `fedml-0.8.7a4/fedml/device/device.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/runner.py` & `fedml-0.8.7a4/fedml/fa/runner.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/fa_server.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/fa_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/fa_client.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/fa_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/server/message_define.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/server/fedml_server_manager.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/server/fedml_aggregator.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/server/server_initializer.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/client_initializer.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/client_launcher.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/message_define.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/fa_local_analyzer.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/fa_local_analyzer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/fedml_client_slave_manager.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/process_group_manager.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/cross_silo/client/fedml_client_master_manager.py` & `fedml-0.8.7a4/fedml/fa/cross_silo/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/frequency_estimation_aggregator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/frequency_estimation_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/intersection_aggregator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/intersection_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/union_aggregator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/union_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/avg_aggregator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/avg_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/k_percentile_element_aggregator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/k_percentile_element_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/heavy_hitter_triehh_aggregator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/heavy_hitter_triehh_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/aggregator/global_analyzer_creator.py` & `fedml-0.8.7a4/fedml/fa/aggregator/global_analyzer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/simulation/sp/client.py` & `fedml-0.8.7a4/fedml/fa/simulation/sp/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/simulation/sp/simulator.py` & `fedml-0.8.7a4/fedml/fa/simulation/sp/simulator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/simulation/utils.py` & `fedml-0.8.7a4/fedml/fa/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/__init__.py` & `fedml-0.8.7a4/fedml/fa/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/utils/trie.py` & `fedml-0.8.7a4/fedml/fa/utils/trie.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/local_analyzer/heavy_hitter_triehh.py` & `fedml-0.8.7a4/fedml/fa/local_analyzer/heavy_hitter_triehh.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/local_analyzer/client_analyzer_creator.py` & `fedml-0.8.7a4/fedml/fa/local_analyzer/client_analyzer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/base_frame/server_aggregator.py` & `fedml-0.8.7a4/fedml/fa/base_frame/server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/base_frame/client_analyzer.py` & `fedml-0.8.7a4/fedml/fa/base_frame/client_analyzer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/data/data_loader.py` & `fedml-0.8.7a4/fedml/fa/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py` & `fedml-0.8.7a4/fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/data/twitter_Sentiment140/data_loader.py` & `fedml-0.8.7a4/fedml/fa/data/twitter_Sentiment140/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/data/utils.py` & `fedml-0.8.7a4/fedml/fa/data/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/data/self_defined_data/data_loader.py` & `fedml-0.8.7a4/fedml/fa/data/self_defined_data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/fa/data/fake_numeric_data/data_loader.py` & `fedml-0.8.7a4/fedml/fa/data/fake_numeric_data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/launch_cross_device.py` & `fedml-0.8.7a4/fedml/launch_cross_device.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/MNIST/mnist_mobile_preprocessor.py` & `fedml-0.8.7a4/fedml/data/MNIST/mnist_mobile_preprocessor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/MNIST/data_loader.py` & `fedml-0.8.7a4/fedml/data/MNIST/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/MNIST/stats.py` & `fedml-0.8.7a4/fedml/data/MNIST/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/lending_club_loan/lending_club_dataset.py` & `fedml-0.8.7a4/fedml/data/lending_club_loan/lending_club_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/lending_club_loan/lending_club_feature_group.py` & `fedml-0.8.7a4/fedml/data/lending_club_loan/lending_club_feature_group.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fed_cifar100/data_loader.py` & `fedml-0.8.7a4/fedml/data/fed_cifar100/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fed_cifar100/dataset.py` & `fedml-0.8.7a4/fedml/data/fed_cifar100/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fed_cifar100/utils.py` & `fedml-0.8.7a4/fedml/data/fed_cifar100/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/FederatedEMNIST/data_loader.py` & `fedml-0.8.7a4/fedml/data/FederatedEMNIST/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cifar100/data_loader.py` & `fedml-0.8.7a4/fedml/data/cifar100/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cifar100/datasets.py` & `fedml-0.8.7a4/fedml/data/cifar100/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/data_loader.py` & `fedml-0.8.7a4/fedml/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/file_operation.py` & `fedml-0.8.7a4/fedml/data/file_operation.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/shakespeare/language_utils.py` & `fedml-0.8.7a4/fedml/data/shakespeare/language_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/shakespeare/data_loader.py` & `fedml-0.8.7a4/fedml/data/shakespeare/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/shakespeare/stats.py` & `fedml-0.8.7a4/fedml/data/shakespeare/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/synthetic_1_1/data_loader.py` & `fedml-0.8.7a4/fedml/data/synthetic_1_1/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/synthetic_1_1/stats.py` & `fedml-0.8.7a4/fedml/data/synthetic_1_1/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/synthetic_1_1/generate_synthetic.py` & `fedml-0.8.7a4/fedml/data/synthetic_1_1/generate_synthetic.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/Landmarks/download_without_tff.py` & `fedml-0.8.7a4/fedml/data/Landmarks/download_without_tff.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/Landmarks/data_loader.py` & `fedml-0.8.7a4/fedml/data/Landmarks/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/Landmarks/datasets.py` & `fedml-0.8.7a4/fedml/data/Landmarks/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/Landmarks/utils.py` & `fedml-0.8.7a4/fedml/data/Landmarks/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/Landmarks/check_download.py` & `fedml-0.8.7a4/fedml/data/Landmarks/check_download.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/Landmarks/download_without_tf.py` & `fedml-0.8.7a4/fedml/data/Landmarks/download_without_tf.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fednlp/base/preprocess/base_example.py` & `fedml-0.8.7a4/fedml/data/fednlp/base/preprocess/base_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fednlp/base/raw_data/partition.py` & `fedml-0.8.7a4/fedml/data/fednlp/base/raw_data/partition.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py` & `fedml-0.8.7a4/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fednlp/base/data_manager/base_data_manager.py` & `fedml-0.8.7a4/fedml/data/fednlp/base/data_manager/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fednlp/base/utils.py` & `fedml-0.8.7a4/fedml/data/fednlp/base/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/NUS_WIDE/nus_wide_dataset.py` & `fedml-0.8.7a4/fedml/data/NUS_WIDE/nus_wide_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/stackoverflow_lr/data_loader.py` & `fedml-0.8.7a4/fedml/data/stackoverflow_lr/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/stackoverflow_lr/dataset.py` & `fedml-0.8.7a4/fedml/data/stackoverflow_lr/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/stackoverflow_lr/utils.py` & `fedml-0.8.7a4/fedml/data/stackoverflow_lr/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fed_shakespeare/data_loader.py` & `fedml-0.8.7a4/fedml/data/fed_shakespeare/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/fed_shakespeare/utils.py` & `fedml-0.8.7a4/fedml/data/fed_shakespeare/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/ImageNet/data_loader.py` & `fedml-0.8.7a4/fedml/data/ImageNet/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/ImageNet/datasets.py` & `fedml-0.8.7a4/fedml/data/ImageNet/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/ImageNet/datasets_hdf5.py` & `fedml-0.8.7a4/fedml/data/ImageNet/datasets_hdf5.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/data_loader_cross_silo.py` & `fedml-0.8.7a4/fedml/data/data_loader_cross_silo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cinic10/data_loader.py` & `fedml-0.8.7a4/fedml/data/cinic10/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cinic10/datasets.py` & `fedml-0.8.7a4/fedml/data/cinic10/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/stackoverflow_nwp/data_loader.py` & `fedml-0.8.7a4/fedml/data/stackoverflow_nwp/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/stackoverflow_nwp/dataset.py` & `fedml-0.8.7a4/fedml/data/stackoverflow_nwp/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/stackoverflow_nwp/utils.py` & `fedml-0.8.7a4/fedml/data/stackoverflow_nwp/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/UCI/data_loader_for_susy_and_ro.py` & `fedml-0.8.7a4/fedml/data/UCI/data_loader_for_susy_and_ro.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/edge_case_examples/data_loader.py` & `fedml-0.8.7a4/fedml/data/edge_case_examples/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/edge_case_examples/datasets.py` & `fedml-0.8.7a4/fedml/data/edge_case_examples/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cifar10/efficient_loader.py` & `fedml-0.8.7a4/fedml/data/cifar10/efficient_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cifar10/data_loader.py` & `fedml-0.8.7a4/fedml/data/cifar10/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cifar10/datasets.py` & `fedml-0.8.7a4/fedml/data/cifar10/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml/data/cifar10/without_reload.py` & `fedml-0.8.7a4/fedml/data/cifar10/without_reload.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml.egg-info/PKG-INFO` & `fedml-0.8.7a4/fedml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml
-Version: 0.8.7a3
+Version: 0.8.7a4
 Summary: A research and production integrated edge-cloud library for federated/distributed machine learning at anywhere at any scale.
 Home-page: https://github.com/FedML-AI/FedML
 Author: FedML Team
 Author-email: ch@fedml.ai
 License: Apache 2.0
 Description: # FedML - The community building and connecting AI anywhere at any scale
```

### Comparing `fedml-0.8.7a3/fedml.egg-info/SOURCES.txt` & `fedml-0.8.7a4/fedml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.7a3/fedml.egg-info/requires.txt` & `fedml-0.8.7a4/fedml.egg-info/requires.txt`

 * *Files identical despite different names*

