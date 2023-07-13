# Comparing `tmp/skyplane_nightly-0.3.2.dev20230711.tar.gz` & `tmp/skyplane_nightly-0.3.2.dev20230712.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyplane_nightly-0.3.2.dev20230711.tar", max compression
+gzip compressed data, was "skyplane_nightly-0.3.2.dev20230712.tar", max compression
```

## Comparing `skyplane_nightly-0.3.2.dev20230711.tar` & `skyplane_nightly-0.3.2.dev20230712.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0    11357 2023-07-11 23:44:11.436443 skyplane_nightly-0.3.2.dev20230711/LICENSE
--rw-r--r--   0        0        0     7221 2023-07-11 23:44:11.436443 skyplane_nightly-0.3.2.dev20230711/README.md
--rw-r--r--   0        0        0     3669 2023-07-11 23:44:58.360827 skyplane_nightly-0.3.2.dev20230711/pyproject.toml
--rw-r--r--   0        0        0      649 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/__init__.py
--rw-r--r--   0        0        0     4331 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/client.py
--rw-r--r--   0        0        0     3040 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/config.py
--rw-r--r--   0        0        0    14841 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/dataplane.py
--rw-r--r--   0        0        0     2081 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/obj_store.py
--rw-r--r--   0        0        0     6750 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/pipeline.py
--rw-r--r--   0        0        0    15091 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/provisioner.py
--rw-r--r--   0        0        0    17597 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/tracker.py
--rw-r--r--   0        0        0    39196 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/transfer_job.py
--rw-r--r--   0        0        0    14790 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/usage.py
--rw-r--r--   0        0        0     6120 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/chunk.py
--rw-r--r--   0        0        0     3317 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli.py
--rw-r--r--   0        0        0    18045 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_cloud.py
--rw-r--r--   0        0        0     1678 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_config.py
--rw-r--r--   0        0        0    27030 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_init.py
--rw-r--r--   0        0        0    24587 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_transfer.py
--rw-r--r--   0        0        0      461 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/__init__.py
--rw-r--r--   0        0        0    23462 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_profile.py
--rw-r--r--   0        0        0     1757 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_query.py
--rw-r--r--   0        0        0     9215 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/provision.py
--rw-r--r--   0        0        0     3100 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/common.py
--rw-r--r--   0        0        0     4678 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/cp_replicate_fallback.py
--rw-r--r--   0        0        0     3071 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/progress_bar.py
--rw-r--r--   0        0        0     1247 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/__init__.py
--rw-r--r--   0        0        0     5908 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_auth.py
--rw-r--r--   0        0        0    11591 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_cloud_provider.py
--rw-r--r--   0        0        0     4315 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_key_manager.py
--rw-r--r--   0        0        0    11509 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_network.py
--rw-r--r--   0        0        0     1606 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_pricing.py
--rw-r--r--   0        0        0     6294 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_server.py
--rw-r--r--   0        0        0     9526 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_auth.py
--rw-r--r--   0        0        0    20681 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_cloud_provider.py
--rw-r--r--   0        0        0     7503 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_server.py
--rw-r--r--   0        0        0     3564 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/cloud_provider.py
--rw-r--r--   0        0        0     2883 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/const_cmds.py
--rw-r--r--   0        0        0    12043 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_auth.py
--rw-r--r--   0        0        0     9355 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_cloud_provider.py
--rw-r--r--   0        0        0     2462 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_key_manager.py
--rw-r--r--   0        0        0     5365 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_network.py
--rw-r--r--   0        0        0     2786 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_pricing.py
--rw-r--r--   0        0        0     5151 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_server.py
--rw-r--r--   0        0        0      211 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
--rw-r--r--   0        0        0        0 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
--rw-r--r--   0        0        0     2242 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/config.py
--rw-r--r--   0        0        0      877 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/constants.py
--rw-r--r--   0        0        0     5353 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
--rw-r--r--   0        0        0      710 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/utils.py
--rw-r--r--   0        0        0    40464 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
--rw-r--r--   0        0        0     5320 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_auth.py
--rw-r--r--   0        0        0     2851 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_provider.py
--rw-r--r--   0        0        0     3522 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_server.py
--rw-r--r--   0        0        0      937 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/key_utils.py
--rw-r--r--   0        0        0    17426 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/server.py
--rw-r--r--   0        0        0    13589 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/config.py
--rw-r--r--   0        0        0     1229 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/config_paths.py
--rw-r--r--   0        0        0        0 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/data/__init__.py
--rw-r--r--   0        0        0    19636 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/data/aws_transfer_costs.csv
--rw-r--r--   0        0        0      617 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/data/vcpu_info.csv
--rw-r--r--   0        0        0     3078 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/exceptions.py
--rw-r--r--   0        0        0      811 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/cert.py
--rw-r--r--   0        0        0     4349 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/chunk_store.py
--rw-r--r--   0        0        0    15655 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon.py
--rw-r--r--   0        0        0    16570 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon_api.py
--rw-r--r--   0        0        0      718 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_onprem.py
--rw-r--r--   0        0        0     5149 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_program.py
--rw-r--r--   0        0        0     1732 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_queue.py
--rw-r--r--   0        0        0        0 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/__init__.py
--rw-r--r--   0        0        0    25487 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_operator.py
--rw-r--r--   0        0        0    10552 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_receiver.py
--rw-r--r--   0        0        0       37 2023-07-11 23:44:58.360827 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway_version.py
--rw-r--r--   0        0        0    13101 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_blob_interface.py
--rw-r--r--   0        0        0     2887 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_storage_account_interface.py
--rw-r--r--   0        0        0    10871 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/cos_interface.py
--rw-r--r--   0        0        0     2010 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/file_system_interface.py
--rw-r--r--   0        0        0    12754 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/gcs_interface.py
--rw-r--r--   0        0        0     5963 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/hdfs_interface.py
--rw-r--r--   0        0        0     3287 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/object_store_interface.py
--rw-r--r--   0        0        0     5644 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/posix_file_interface.py
--rw-r--r--   0        0        0     3606 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/r2_interface.py
--rw-r--r--   0        0        0    11595 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/s3_interface.py
--rw-r--r--   0        0        0     2569 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/storage_interface.py
--rw-r--r--   0        0        0    23858 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/planner.py
--rw-r--r--   0        0        0    18157 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver.py
--rw-r--r--   0        0        0     6467 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ilp.py
--rw-r--r--   0        0        0     1996 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ron.py
--rw-r--r--   0        0        0     7920 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/topology.py
--rw-r--r--   0        0        0      846 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/cache.py
--rw-r--r--   0        0        0      617 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/definitions.py
--rw-r--r--   0        0        0     2494 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/fn.py
--rw-r--r--   0        0        0     1881 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/generator.py
--rw-r--r--   0        0        0     1386 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/imports.py
--rw-r--r--   0        0        0     2131 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/logger.py
--rw-r--r--   0        0        0     1447 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/networking_tools.py
--rw-r--r--   0        0        0     3162 2023-07-11 23:44:11.460443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/path.py
--rw-r--r--   0        0        0     1160 2023-07-11 23:44:11.460443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/retry.py
--rw-r--r--   0        0        0      612 2023-07-11 23:44:11.460443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/timer.py
--rw-r--r--   0        0        0    10493 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230711/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-12 23:44:26.102683 skyplane_nightly-0.3.2.dev20230712/LICENSE
+-rw-r--r--   0        0        0     7221 2023-07-12 23:44:26.102683 skyplane_nightly-0.3.2.dev20230712/README.md
+-rw-r--r--   0        0        0     3669 2023-07-12 23:45:24.195245 skyplane_nightly-0.3.2.dev20230712/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/__init__.py
+-rw-r--r--   0        0        0     4331 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/client.py
+-rw-r--r--   0        0        0     3040 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/config.py
+-rw-r--r--   0        0        0    14841 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/dataplane.py
+-rw-r--r--   0        0        0     2081 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/obj_store.py
+-rw-r--r--   0        0        0     6750 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/pipeline.py
+-rw-r--r--   0        0        0    15091 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/provisioner.py
+-rw-r--r--   0        0        0    17597 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/tracker.py
+-rw-r--r--   0        0        0    38945 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/transfer_job.py
+-rw-r--r--   0        0        0    14790 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/api/usage.py
+-rw-r--r--   0        0        0     6120 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/chunk.py
+-rw-r--r--   0        0        0     3317 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli.py
+-rw-r--r--   0        0        0    18045 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_cloud.py
+-rw-r--r--   0        0        0     1678 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_config.py
+-rw-r--r--   0        0        0    27030 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_init.py
+-rw-r--r--   0        0        0    24587 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_transfer.py
+-rw-r--r--   0        0        0      461 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/__init__.py
+-rw-r--r--   0        0        0    23462 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/cli_profile.py
+-rw-r--r--   0        0        0     1757 2023-07-12 23:44:26.118685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/cli_query.py
+-rw-r--r--   0        0        0     9215 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/provision.py
+-rw-r--r--   0        0        0     3100 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/impl/common.py
+-rw-r--r--   0        0        0     4678 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/impl/cp_replicate_fallback.py
+-rw-r--r--   0        0        0     3071 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/cli/impl/progress_bar.py
+-rw-r--r--   0        0        0     1247 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/__init__.py
+-rw-r--r--   0        0        0     5908 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_auth.py
+-rw-r--r--   0        0        0    11591 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_cloud_provider.py
+-rw-r--r--   0        0        0     4315 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_key_manager.py
+-rw-r--r--   0        0        0    11509 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_network.py
+-rw-r--r--   0        0        0     1606 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_pricing.py
+-rw-r--r--   0        0        0     6294 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_server.py
+-rw-r--r--   0        0        0     9526 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/azure/azure_auth.py
+-rw-r--r--   0        0        0    20681 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/azure/azure_cloud_provider.py
+-rw-r--r--   0        0        0     7503 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/azure/azure_server.py
+-rw-r--r--   0        0        0     3564 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/cloud_provider.py
+-rw-r--r--   0        0        0     2883 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/const_cmds.py
+-rw-r--r--   0        0        0    12043 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_auth.py
+-rw-r--r--   0        0        0     9355 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_cloud_provider.py
+-rw-r--r--   0        0        0     2462 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_key_manager.py
+-rw-r--r--   0        0        0     6288 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_network.py
+-rw-r--r--   0        0        0     2786 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_pricing.py
+-rw-r--r--   0        0        0     5151 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_server.py
+-rw-r--r--   0        0        0      211 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
+-rw-r--r--   0        0        0        0 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
+-rw-r--r--   0        0        0     2242 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/config.py
+-rw-r--r--   0        0        0      877 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/constants.py
+-rw-r--r--   0        0        0     5353 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
+-rw-r--r--   0        0        0      710 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/utils.py
+-rw-r--r--   0        0        0    40464 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
+-rw-r--r--   0        0        0     5320 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibmcloud_auth.py
+-rw-r--r--   0        0        0     2851 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibmcloud_provider.py
+-rw-r--r--   0        0        0     3522 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibmcloud_server.py
+-rw-r--r--   0        0        0      937 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/key_utils.py
+-rw-r--r--   0        0        0    17426 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/compute/server.py
+-rw-r--r--   0        0        0    13589 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/config.py
+-rw-r--r--   0        0        0     1229 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/config_paths.py
+-rw-r--r--   0        0        0        0 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/data/__init__.py
+-rw-r--r--   0        0        0    19636 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/data/aws_transfer_costs.csv
+-rw-r--r--   0        0        0      617 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/data/vcpu_info.csv
+-rw-r--r--   0        0        0     3078 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/exceptions.py
+-rw-r--r--   0        0        0      811 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/cert.py
+-rw-r--r--   0        0        0     4349 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/chunk_store.py
+-rw-r--r--   0        0        0    15655 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_daemon.py
+-rw-r--r--   0        0        0    16570 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_daemon_api.py
+-rw-r--r--   0        0        0      718 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_onprem.py
+-rw-r--r--   0        0        0     5149 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_program.py
+-rw-r--r--   0        0        0     1732 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_queue.py
+-rw-r--r--   0        0        0        0 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/operators/__init__.py
+-rw-r--r--   0        0        0    25487 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/operators/gateway_operator.py
+-rw-r--r--   0        0        0    10552 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/operators/gateway_receiver.py
+-rw-r--r--   0        0        0       37 2023-07-12 23:45:24.191244 skyplane_nightly-0.3.2.dev20230712/skyplane/gateway_version.py
+-rw-r--r--   0        0        0    13101 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/azure_blob_interface.py
+-rw-r--r--   0        0        0     2887 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/azure_storage_account_interface.py
+-rw-r--r--   0        0        0    10871 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/cos_interface.py
+-rw-r--r--   0        0        0     2010 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/file_system_interface.py
+-rw-r--r--   0        0        0    12754 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/gcs_interface.py
+-rw-r--r--   0        0        0     5963 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/hdfs_interface.py
+-rw-r--r--   0        0        0     3287 2023-07-12 23:44:26.122685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/object_store_interface.py
+-rw-r--r--   0        0        0     5644 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/posix_file_interface.py
+-rw-r--r--   0        0        0     3606 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/r2_interface.py
+-rw-r--r--   0        0        0    11595 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/s3_interface.py
+-rw-r--r--   0        0        0     2569 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/storage_interface.py
+-rw-r--r--   0        0        0    23858 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/planner/planner.py
+-rw-r--r--   0        0        0    18157 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/planner/solver.py
+-rw-r--r--   0        0        0     6467 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/planner/solver_ilp.py
+-rw-r--r--   0        0        0     1996 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/planner/solver_ron.py
+-rw-r--r--   0        0        0     7920 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/planner/topology.py
+-rw-r--r--   0        0        0      846 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/cache.py
+-rw-r--r--   0        0        0      617 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/definitions.py
+-rw-r--r--   0        0        0     2494 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/fn.py
+-rw-r--r--   0        0        0     1881 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/generator.py
+-rw-r--r--   0        0        0     1386 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/imports.py
+-rw-r--r--   0        0        0     2131 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/logger.py
+-rw-r--r--   0        0        0     1447 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/networking_tools.py
+-rw-r--r--   0        0        0     3162 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/path.py
+-rw-r--r--   0        0        0     1160 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/retry.py
+-rw-r--r--   0        0        0      612 2023-07-12 23:44:26.126685 skyplane_nightly-0.3.2.dev20230712/skyplane/utils/timer.py
+-rw-r--r--   0        0        0    10493 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230712/PKG-INFO
```

### Comparing `skyplane_nightly-0.3.2.dev20230711/LICENSE` & `skyplane_nightly-0.3.2.dev20230712/LICENSE`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/README.md` & `skyplane_nightly-0.3.2.dev20230712/README.md`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/pyproject.toml` & `skyplane_nightly-0.3.2.dev20230712/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "skyplane-nightly"
 packages = [{ include = "skyplane" }]
-version = "0.3.2.dev20230711"
+version = "0.3.2.dev20230712"
 description = "Skyplane efficiently transports data between cloud regions and providers."
 authors = ["Skyplane authors <skyplaneproject@gmail.com>"]
 license = "Apache-2.0"
 homepage = "https://skyplane.org/"
 repository = "https://github.com/skyplane-project/skyplane"
 documentation = "https://skyplane.org/"
 readme = "README.md"
```

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/__init__.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/__init__.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/client.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/client.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/config.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/dataplane.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/dataplane.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/obj_store.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/obj_store.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/pipeline.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/provisioner.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/provisioner.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/tracker.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/tracker.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/transfer_job.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/transfer_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,37 +327,30 @@
         :type transfer_pair_generator: Generator
         """
         multipart_send_queue: Queue[TransferPair] = Queue()
         multipart_chunk_queue: Queue[GatewayMessage] = Queue()
         multipart_exit_event = threading.Event()
         multipart_chunk_threads = []
 
-        # TODO: remove after azure multipart implemented
-        azure_dest = any([dst_iface.provider == "azure" for dst_iface in self.dst_ifaces])
-
         # start chunking threads
-        if not azure_dest and self.transfer_config.multipart_enabled:
+        if self.transfer_config.multipart_enabled:
             for _ in range(self.concurrent_multipart_chunk_threads):
                 t = threading.Thread(
                     target=self._run_multipart_chunk_thread,
                     args=(multipart_exit_event, multipart_send_queue, multipart_chunk_queue),
                     daemon=False,
                 )
                 t.start()
                 multipart_chunk_threads.append(t)
 
         # begin chunking loop
         for transfer_pair in transfer_pair_generator:
             # print("transfer_pair", transfer_pair.src_obj.key, transfer_pair.dst_objs)
             src_obj = transfer_pair.src_obj
-            if (
-                not azure_dest
-                and self.transfer_config.multipart_enabled
-                and src_obj.size > self.transfer_config.multipart_threshold_mb * MB
-            ):
+            if self.transfer_config.multipart_enabled and src_obj.size > self.transfer_config.multipart_threshold_mb * MB:
                 multipart_send_queue.put(transfer_pair)
             else:
                 if transfer_pair.src_obj.size == 0:
                     logger.fs.debug(f"Skipping empty object {src_obj.key}")
                     continue
                 yield GatewayMessage(
                     chunk=Chunk(
```

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/api/usage.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/api/usage.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/chunk.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/chunk.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_cloud.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_cloud.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_config.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_init.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
         logger.debug(f"Found existing configuration file at {config_path}, loading")
         cloud_config = SkyplaneConfig.load_config(config_path)
     else:
         cloud_config = SkyplaneConfig.default_config()
 
     # load AWS config
     if not (reinit_azure or reinit_gcp or reinit_ibm):
-        typer.secho("\n(1) configuring AWS:", fg="yellow", bold=True)
+        typer.secho("\n(1) Configuring AWS:", fg="yellow", bold=True)
         if not disable_config_aws:
             cloud_config = load_aws_config(cloud_config, non_interactive=non_interactive)
 
     # load Azure config
     if not (reinit_gcp or reinit_ibm):
         if reinit_azure:
             typer.secho("\nConfiguring Azure:", fg="yellow", bold=True)
```

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_transfer.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/cli_transfer.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_profile.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/cli_profile.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_query.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/cli_query.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/provision.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/experiments/provision.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/common.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/impl/common.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/cp_replicate_fallback.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/impl/cp_replicate_fallback.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/progress_bar.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/cli/impl/progress_bar.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/__init__.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_auth.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_key_manager.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_network.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_network.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_pricing.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_server.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/aws/aws_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_auth.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/azure/azure_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/azure/azure_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_server.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/azure/azure_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/const_cmds.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/const_cmds.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_auth.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_key_manager.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_network.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_network.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,25 +38,47 @@
 
     @imports.inject("googleapiclient.errors", pip_extra="gcp")
     def delete_network(errors, self):
         """
         Delete VPC. This might error our in some cases.
         """
         compute = self.auth.get_gcp_client()
+
+        # delete firewall rules
+        self.delete_firewall_rules()
+
+        # delete network
         request = compute.networks().delete(project=self.auth.project_id, network=self.vpc_name)
         try:
             delete_vpc_response = request.execute()
             self.auth.wait_for_operation_to_complete("global", delete_vpc_response)
         except errors.HttpError as e:
             logger.fs.warn(
                 f"Unable to delete network. Ensure no active firewall rules acting upon the {self.vpc_name} VPC. Ensure no instances provisioned in the VPC "
             )
             logger.fs.error(e)
 
     @imports.inject("googleapiclient.errors", pip_extra="gcp")
+    def delete_firewall_rules(errors, self):
+        # Get the firewall rules in the network
+        compute = self.auth.get_gcp_client()
+        request = compute.firewalls().list(project=self.auth.project_id)
+        response = request.execute()
+        if "items" not in response:
+            # no firewall rules found
+            return
+
+        # Delete each firewall rule
+        for rule in response["items"]:
+            if rule["network"] == f"https://www.googleapis.com/compute/v1/projects/{self.auth.project_id}/global/networks/{self.vpc_name}":
+                rule_name = rule["name"]
+                print(f"Deleting firewall rule: {rule_name}")
+                compute.firewalls().delete(project=self.auth.project_id, firewall=rule_name).execute()
+
+    @imports.inject("googleapiclient.errors", pip_extra="gcp")
     def get_firewall_rule(errors, self, firewall_rule_name):
         compute = self.auth.get_gcp_client()
         try:
             return compute.firewalls().get(project=self.auth.project_id, firewall=firewall_rule_name).execute()
         except errors.HttpError as e:
             if e.resp.status == 404:
                 return None
```

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_pricing.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_server.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/gcp/gcp_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/config.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/constants.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/constants.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/utils.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/utils.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_auth.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibmcloud_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_provider.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibmcloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_server.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/ibmcloud/ibmcloud_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/key_utils.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/key_utils.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/server.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/compute/server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/config.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/config_paths.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/config_paths.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/data/aws_transfer_costs.csv` & `skyplane_nightly-0.3.2.dev20230712/skyplane/data/aws_transfer_costs.csv`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/data/vcpu_info.csv` & `skyplane_nightly-0.3.2.dev20230712/skyplane/data/vcpu_info.csv`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/exceptions.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/cert.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/cert.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/chunk_store.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/chunk_store.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_daemon.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon_api.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_daemon_api.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_onprem.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_onprem.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_program.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_program.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_queue.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/gateway_queue.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_operator.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/operators/gateway_operator.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_receiver.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/gateway/operators/gateway_receiver.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_blob_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/azure_blob_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_storage_account_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/azure_storage_account_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/cos_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/cos_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/file_system_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/file_system_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/gcs_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/gcs_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/hdfs_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/hdfs_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/object_store_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/object_store_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/posix_file_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/posix_file_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/r2_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/r2_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/s3_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/s3_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/storage_interface.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/obj_store/storage_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/planner.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/planner/planner.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/planner/solver.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ilp.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/planner/solver_ilp.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ron.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/planner/solver_ron.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/topology.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/planner/topology.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/cache.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/cache.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/definitions.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/fn.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/fn.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/generator.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/generator.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/imports.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/imports.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/logger.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/logger.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/networking_tools.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/networking_tools.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/path.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/path.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/retry.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/retry.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/timer.py` & `skyplane_nightly-0.3.2.dev20230712/skyplane/utils/timer.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230711/PKG-INFO` & `skyplane_nightly-0.3.2.dev20230712/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyplane-nightly
-Version: 0.3.2.dev20230711
+Version: 0.3.2.dev20230712
 Summary: Skyplane efficiently transports data between cloud regions and providers.
 Home-page: https://skyplane.org/
 License: Apache-2.0
 Author: Skyplane authors
 Author-email: skyplaneproject@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

