# Comparing `tmp/langport-0.3.0.tar.gz` & `tmp/langport-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.3.0.tar", last modified: Fri Jun 30 07:29:25 2023, max compression
+gzip compressed data, was "langport-0.3.1.tar", last modified: Fri Jul 14 07:43:15 2023, max compression
```

## Comparing `langport-0.3.0.tar` & `langport-0.3.1.tar`

### file list

```diff
@@ -1,143 +1,145 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.0/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5811 2023-06-30 07:29:25.437850 langport-0.3.0/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5311 2023-06-30 05:10:13.000000 langport-0.3.0/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.0/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.3.0/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.0/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.0/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.0/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.3.0/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.0/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.0/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6133 2023-06-30 07:16:30.000000 langport-0.3.0/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-06-30 07:13:56.000000 langport-0.3.0/langport/data/conversation/settings/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/mpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-06-21 13:48:49.000000 langport-0.3.0/langport/data/conversation/settings/wizardlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.0/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.0/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-06-21 13:45:50.000000 langport-0.3.0/langport/model/adapters/baichuan.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-06-30 07:16:13.000000 langport-0.3.0/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/codegen.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/starcoder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/text2vec.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-06-21 13:47:17.000000 langport-0.3.0/langport/model/adapters/wizardlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5000 2023-06-25 16:41:24.000000 langport-0.3.0/langport/model/executor/generation/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16189 2023-06-25 16:41:24.000000 langport-0.3.0/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-06-21 04:13:56.000000 langport-0.3.0/langport/model/executor/generation/optimum.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2110 2023-06-18 13:11:45.000000 langport-0.3.0/langport/model/executor/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7679 2023-06-30 07:18:19.000000 langport-0.3.0/langport/model/executor/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1567 2023-06-21 14:56:58.000000 langport-0.3.0/langport/model/executor/optimum.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-30 05:32:15.000000 langport-0.3.0/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-30 07:22:43.000000 langport-0.3.0/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.0/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.0/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/monkey_patch_non_inplace.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.0/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.0/langport/protocol/huggingface_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.3.0/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.0/langport/protocol/tabby_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.3.0/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.3.0/langport/routers/gateway/common.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16286 2023-06-30 05:36:09.000000 langport-0.3.0/langport/routers/gateway/openai_compatible.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.0/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-30 05:34:00.000000 langport-0.3.0/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.0/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/cluster_monitor.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/cluster_monitor_app.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/graphite_feeder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/huggingface_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-25 16:41:24.000000 langport-0.3.0/langport/service/gateway/openai_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/tabby_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2614 2023-06-30 07:23:01.000000 langport-0.3.0/langport/service/server/generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2911 2023-06-18 13:11:45.000000 langport-0.3.0/langport/service/server/ggml_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2582 2023-06-21 04:13:56.000000 langport-0.3.0/langport/service/server/optimum_generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-06-30 05:09:13.000000 langport-0.3.0/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.3.0/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.0/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.0/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.3.0/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-06-25 16:41:24.000000 langport-0.3.0/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.3.0/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.3.0/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5811 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4473 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-06-21 04:13:56.000000 langport-0.3.0/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-30 07:29:25.437850 langport-0.3.0/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.1/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5865 2023-07-14 07:43:15.120559 langport-0.3.1/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5365 2023-07-14 07:42:48.000000 langport-0.3.1/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.1/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.3.1/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.1/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.1/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.1/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.3.1/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.1/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.1/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6133 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/settings/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      286 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/settings/ningyu.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-07-14 07:42:48.000000 langport-0.3.1/langport/data/conversation/settings/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.1/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.1/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.1/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/baichuan.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      840 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/ningyu.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/adapters/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7287 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-07-13 17:09:49.000000 langport-0.3.1/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.1/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5276 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/generation/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    20845 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/generation/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2341 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7679 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1567 2023-07-14 07:42:48.000000 langport-0.3.1/langport/model/executor/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-30 05:32:15.000000 langport-0.3.1/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-30 07:22:43.000000 langport-0.3.1/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.1/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.1/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.1/langport/model/monkey_patch_non_inplace.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.1/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.1/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4665 2023-07-14 07:42:48.000000 langport-0.3.1/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.1/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2948 2023-07-14 07:42:48.000000 langport-0.3.1/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.3.1/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16721 2023-07-14 07:42:48.000000 langport-0.3.1/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.1/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.1/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3580 2023-07-14 07:42:48.000000 langport-0.3.1/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.116559 langport-0.3.1/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.1/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-25 16:41:24.000000 langport-0.3.1/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.1/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2614 2023-07-14 07:42:48.000000 langport-0.3.1/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3034 2023-07-14 07:42:48.000000 langport-0.3.1/langport/service/server/ggml_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2582 2023-07-14 07:42:48.000000 langport-0.3.1/langport/service/server/optimum_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-07-14 07:42:48.000000 langport-0.3.1/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.3.1/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.1/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.1/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.3.1/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-07-14 07:42:48.000000 langport-0.3.1/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.120559 langport-0.3.1/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.1/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.3.1/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3175 2023-07-14 07:42:48.000000 langport-0.3.1/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-14 07:43:15.112559 langport-0.3.1/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5865 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4553 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-07-14 07:43:15.000000 langport-0.3.1/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-07-14 07:42:48.000000 langport-0.3.1/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-07-14 07:43:15.120559 langport-0.3.1/setup.cfg
```

### Comparing `langport-0.3.0/LICENSE` & `langport-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/PKG-INFO` & `langport-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.3.0
+Version: 0.3.1
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -67,14 +67,15 @@
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
 - [2023/05/22] New distributed architecture.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.3.0 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.3.1 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
 Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -20,41 +20,42 @@
 RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
 LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
 LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
 ## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
 V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
 server, and the following figure shows the Queries Per Second (QPS) and Tokens
 Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18]
-Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09]
-Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
-worker support. - [2023/06/01] Add HuggingFace text generation API support. -
-[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
-script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
-inference supported. - [2023/05/10] Langport project started. ## Install ###
-Method 1: With pip ```bash pip install langport ``` or: ```bash pip install
-git+https://github.com/vtuber-plan/langport.git ``` If you need ggml generation
-worker, use this command: ```bash pip install langport[ggml] ``` If you wanna
-use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From
-source 1. Clone this repository ```bash git clone https://github.com/vtuber-
-plan/langport.git cd langport ``` 2. Install the Package ```bash pip install --
-upgrade pip pip install -e . ``` ## Start the server It is simple to start a
-single node chat API service: ``` bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  python -
-m langport.service.gateway.openai_api ``` If you need the embeddings API or
-other features, you can deploy a distributed inference cluster: ``` bash python
--m langport.service.server.dummy_worker --port 21001 python -
-m langport.service.server.generation_worker --model-path  --neighbors http://
-localhost:21001 python -m langport.service.server.embedding_worker --model-path
---neighbors http://localhost:21001 python -
-m langport.service.gateway.openai_api --controller-address http://localhost:
-21001 ``` In practice, the gateway can connect to any node to distribute
-inference tasks: ``` bash python -m langport.service.server.dummy_worker --port
-21001 python -m langport.service.server.generation_worker --port 21002 --model-
-path  --neighbors http://localhost:21001 python -
+settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/07/13]
+Support generation logprobs parameter. - [2023/06/18] Add ggml (llama.cpp
+gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add LLama.cpp worker
+support. - [2023/06/01] Add HuggingFace Bert embedding worker support. - [2023/
+06/01] Add HuggingFace text generation API support. - [2023/06/01] Add tabby
+API support. - [2023/05/23] Add chat throughput test script. - [2023/05/22] New
+distributed architecture. - [2023/05/14] Batch inference supported. - [2023/05/
+10] Langport project started. ## Install ### Method 1: With pip ```bash pip
+install langport ``` or: ```bash pip install git+https://github.com/vtuber-
+plan/langport.git ``` If you need ggml generation worker, use this command:
+```bash pip install langport[ggml] ``` If you wanna use GPU: ```bash
+CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1. Clone
+this repository ```bash git clone https://github.com/vtuber-plan/langport.git
+cd langport ``` 2. Install the Package ```bash pip install --upgrade pip pip
+install -e . ``` ## Start the server It is simple to start a single node chat
+API service: ``` bash python -m langport.service.server.generation_worker --
+port 21001 --model-path  python -m langport.service.gateway.openai_api ``` If
+you need the embeddings API or other features, you can deploy a distributed
+inference cluster: ``` bash python -m langport.service.server.dummy_worker --
+port 21001 python -m langport.service.server.generation_worker --model-path  --
+neighbors http://localhost:21001 python -
+m langport.service.server.embedding_worker --model-path  --neighbors http://
+localhost:21001 python -m langport.service.gateway.openai_api --controller-
+address http://localhost:21001 ``` In practice, the gateway can connect to any
+node to distribute inference tasks: ``` bash python -
+m langport.service.server.dummy_worker --port 21001 python -
+m langport.service.server.generation_worker --port 21002 --model-path  --
+neighbors http://localhost:21001 python -
 m langport.service.server.generation_worker --port 21003 --model-path  --
 neighbors http://localhost:21001 http://localhost:21002 python -
 m langport.service.server.generation_worker --port 21004 --model-path  --
 neighbors http://localhost:21001 http://localhost:21003 python -
 m langport.service.server.generation_worker --port 21005 --model-path  --
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
```

### Comparing `langport-0.3.0/README.md` & `langport-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
 - [2023/05/22] New distributed architecture.
```

#### html2text {}

```diff
@@ -13,41 +13,42 @@
 RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
 LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
 LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
 ## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
 V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
 server, and the following figure shows the Queries Per Second (QPS) and Tokens
 Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18]
-Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09]
-Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
-worker support. - [2023/06/01] Add HuggingFace text generation API support. -
-[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
-script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
-inference supported. - [2023/05/10] Langport project started. ## Install ###
-Method 1: With pip ```bash pip install langport ``` or: ```bash pip install
-git+https://github.com/vtuber-plan/langport.git ``` If you need ggml generation
-worker, use this command: ```bash pip install langport[ggml] ``` If you wanna
-use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From
-source 1. Clone this repository ```bash git clone https://github.com/vtuber-
-plan/langport.git cd langport ``` 2. Install the Package ```bash pip install --
-upgrade pip pip install -e . ``` ## Start the server It is simple to start a
-single node chat API service: ``` bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  python -
-m langport.service.gateway.openai_api ``` If you need the embeddings API or
-other features, you can deploy a distributed inference cluster: ``` bash python
--m langport.service.server.dummy_worker --port 21001 python -
-m langport.service.server.generation_worker --model-path  --neighbors http://
-localhost:21001 python -m langport.service.server.embedding_worker --model-path
---neighbors http://localhost:21001 python -
-m langport.service.gateway.openai_api --controller-address http://localhost:
-21001 ``` In practice, the gateway can connect to any node to distribute
-inference tasks: ``` bash python -m langport.service.server.dummy_worker --port
-21001 python -m langport.service.server.generation_worker --port 21002 --model-
-path  --neighbors http://localhost:21001 python -
+settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/07/13]
+Support generation logprobs parameter. - [2023/06/18] Add ggml (llama.cpp
+gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add LLama.cpp worker
+support. - [2023/06/01] Add HuggingFace Bert embedding worker support. - [2023/
+06/01] Add HuggingFace text generation API support. - [2023/06/01] Add tabby
+API support. - [2023/05/23] Add chat throughput test script. - [2023/05/22] New
+distributed architecture. - [2023/05/14] Batch inference supported. - [2023/05/
+10] Langport project started. ## Install ### Method 1: With pip ```bash pip
+install langport ``` or: ```bash pip install git+https://github.com/vtuber-
+plan/langport.git ``` If you need ggml generation worker, use this command:
+```bash pip install langport[ggml] ``` If you wanna use GPU: ```bash
+CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1. Clone
+this repository ```bash git clone https://github.com/vtuber-plan/langport.git
+cd langport ``` 2. Install the Package ```bash pip install --upgrade pip pip
+install -e . ``` ## Start the server It is simple to start a single node chat
+API service: ``` bash python -m langport.service.server.generation_worker --
+port 21001 --model-path  python -m langport.service.gateway.openai_api ``` If
+you need the embeddings API or other features, you can deploy a distributed
+inference cluster: ``` bash python -m langport.service.server.dummy_worker --
+port 21001 python -m langport.service.server.generation_worker --model-path  --
+neighbors http://localhost:21001 python -
+m langport.service.server.embedding_worker --model-path  --neighbors http://
+localhost:21001 python -m langport.service.gateway.openai_api --controller-
+address http://localhost:21001 ``` In practice, the gateway can connect to any
+node to distribute inference tasks: ``` bash python -
+m langport.service.server.dummy_worker --port 21001 python -
+m langport.service.server.generation_worker --port 21002 --model-path  --
+neighbors http://localhost:21001 python -
 m langport.service.server.generation_worker --port 21003 --model-path  --
 neighbors http://localhost:21001 http://localhost:21002 python -
 m langport.service.server.generation_worker --port 21004 --model-path  --
 neighbors http://localhost:21001 http://localhost:21003 python -
 m langport.service.server.generation_worker --port 21005 --model-path  --
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
```

### Comparing `langport-0.3.0/langport/constants.py` & `langport-0.3.1/langport/constants.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/core/base_node.py` & `langport-0.3.1/langport/core/base_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/core/cluster_node.py` & `langport-0.3.1/langport/core/cluster_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/core/cluster_worker.py` & `langport-0.3.1/langport/core/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/data/conversation/__init__.py` & `langport-0.3.1/langport/data/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/data/conversation/conversation_settings.py` & `langport-0.3.1/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/baichuan.py` & `langport-0.3.1/langport/model/adapters/baichuan.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/baize.py` & `langport-0.3.1/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/bard.py` & `langport-0.3.1/langport/model/adapters/bard.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/billa.py` & `langport-0.3.1/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/chatglm.py` & `langport-0.3.1/langport/model/adapters/chatglm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/chatgpt.py` & `langport-0.3.1/langport/model/adapters/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/claude.py` & `langport-0.3.1/langport/model/adapters/claude.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/dolly_v2.py` & `langport-0.3.1/langport/model/adapters/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/falcon.py` & `langport-0.3.1/langport/model/adapters/falcon.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/koala.py` & `langport-0.3.1/langport/model/adapters/koala.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/oasst_pythia.py` & `langport-0.3.1/langport/model/adapters/oasst_pythia.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/openbuddy.py` & `langport-0.3.1/langport/model/adapters/openbuddy.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/phoenix.py` & `langport-0.3.1/langport/model/adapters/phoenix.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/rwkv.py` & `langport-0.3.1/langport/model/adapters/rwkv.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/stable_lm.py` & `langport-0.3.1/langport/model/adapters/stable_lm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/vicuna.py` & `langport-0.3.1/langport/model/adapters/vicuna.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/adapters/wizardlm.py` & `langport-0.3.1/langport/model/adapters/wizardlm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/compression.py` & `langport-0.3.1/langport/model/compression.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,19 @@
             self.weight = compress(weight.data.to(device), default_compression_config)
         else:
             self.weight = weight
         self.bias = bias
 
     def forward(self, input: Tensor) -> Tensor:
         weight = decompress(self.weight, default_compression_config)
-        return F.linear(input.to(weight.dtype), weight, self.bias)
+        if self.bias is not None:
+            bias = self.bias.to(weight.dtype)
+        else:
+            bias = self.bias
+        return F.linear(input.to(weight.dtype), weight, bias)
 
 
 def compress_module(module, target_device):
     for attr_str in dir(module):
         target_attr = getattr(module, attr_str)
         if type(target_attr) == torch.nn.Linear:
             setattr(
@@ -134,15 +138,14 @@
             )
     apply_compressed_weight(model, compressed_state_dict, device)
 
     model.to(device)
 
     return model, tokenizer
 
-
 def compress(tensor, config):
     """Simulate group-wise quantization."""
     if not config.enabled:
         return tensor
 
     group_size, num_bits, group_dim, symmetric = (
         config.group_size,
@@ -187,15 +190,14 @@
         scale = B / (mx - mn)
         data = data - mn
         data.mul_(scale)
 
         data = data.clamp_(0, B).round_().to(torch.uint8)
         return data, mn, scale, original_shape
 
-
 def decompress(packed_data, config):
     """Simulate group-wise dequantization."""
     if not config.enabled:
         return packed_data
 
     group_size, num_bits, group_dim, symmetric = (
         config.group_size,
```

### Comparing `langport-0.3.0/langport/model/executor/base.py` & `langport-0.3.1/langport/model/executor/base.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/embedding/__init__.py` & `langport-0.3.1/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/embedding/huggingface.py` & `langport-0.3.1/langport/model/executor/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/generation/__init__.py` & `langport-0.3.1/langport/model/executor/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/generation/chatgpt.py` & `langport-0.3.1/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/generation/ggml.py` & `langport-0.3.1/langport/model/executor/generation/ggml.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,22 +24,24 @@
             output = task.prompt
         else:
             tokens = tokenizer.encode(task.prompt)
             prompt_length = len(tokens)
             output_ids = []
 
             # Compatible with some models
-            top_k = 40 if task.top_k <= 1 else task.top_k
-            repetition_penalty = 1.17647 if task.repetition_penalty == 0.0 else task.repetition_penalty
+            top_k = 10 if task.top_k <= 1 else task.top_k
+            repetition_penalty = 1.01 if task.repetition_penalty == 0.0 else task.repetition_penalty
+            model.config.max_new_tokens = task.max_tokens
 
             finish_reason = "stop"
             n_tokens = 0
             for token in model.generate(
-                            tokens, top_k=top_k, top_p=task.top_p, batch_size=512,
-                            temperature=task.temperature, repetition_penalty=repetition_penalty):
+                            tokens, top_k=top_k, top_p=task.top_p, batch_size=model.config.batch_size,
+                            threads=model.config.threads, temperature=task.temperature, 
+                            last_n_tokens=256, repetition_penalty=repetition_penalty, reset=True):
                 n_tokens += 1
                 output_ids.append(token)
                 if n_tokens == task.max_tokens:
                     output = tokenizer.decode(output_ids)
                     finish_reason = "length"
                     yield GenerationWorkerResult(
                         task_id=task.task_id,
@@ -90,25 +92,29 @@
 class GgmlGenerationExecutor(GgmlExecutor):
     def __init__(
         self,
         model_name: str,
         model_path: str,
         context_length: int,
         gpu_layers: int,
+        chunk_size: int,
+        threads: int,
         model_type: str = "llama",
         lib: Optional[str] = None,
     ) -> None:
         n_gpu = 1 if gpu_layers > 0 else 0
         super(GgmlGenerationExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device="cpu",
             num_gpus=n_gpu,
             max_gpu_memory=None,
             gpu_layers=gpu_layers,
+            chunk_size=chunk_size,
+            threads=threads,
             lib=lib,
             model_type=model_type,
         )
         self.n_ctx = context_length
         self.adapter, self.model, self.tokenizer = self.load_model(model_path, from_pretrained_kwargs={})
         self.lock = threading.Lock()
```

### Comparing `langport-0.3.0/langport/model/executor/generation/huggingface.py` & `langport-0.3.1/langport/model/executor/generation/huggingface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Any, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Union
 from langport.model.executor.generation import BaseStreamer
 
 from langport.model.executor.huggingface import HuggingfaceExecutor
 
 from langport.protocol.worker_protocol import (
     BaseWorkerResult,
     GenerationTask,
+    GenerationWorkerLogprobs,
     GenerationWorkerResult,
     UsageInfo,
 )
 
 import torch
 
-from transformers import PreTrainedModel, PreTrainedTokenizerBase
+from transformers import PreTrainedModel, PreTrainedTokenizer
 from transformers.generation.logits_process import (
     LogitsProcessor,
     LogitsProcessorList,
     TemperatureLogitsWarper,
     RepetitionPenaltyLogitsProcessor,
     TopPLogitsWarper,
     TopKLogitsWarper,
@@ -26,14 +27,20 @@
 from cachetools import LRUCache, TTLCache
 from asyncache import cached
 
 from typing import Optional
 
 import torch
 
+def token_to_unicode(token: str) -> str:
+    utf8_bytes = token.encode("utf-8")
+    # Convert the bytes to a string with \\x escape sequences
+    escaped_bytes = "".join([f"\\x{b:02x}" for b in utf8_bytes])
+    return escaped_bytes
+
 @cached(LRUCache(maxsize=64))
 def prepare_logits_processor(
     temperature: float, repetition_penalty: float, top_p: float, top_k: int
 ) -> LogitsProcessorList:
     processor_list = LogitsProcessorList()
     # TemperatureLogitsWarper doesn't accept 0.0, 1.0 makes it a no-op so we skip two cases.
     if temperature >= 1e-5 and temperature != 1.0:
@@ -44,15 +51,15 @@
         processor_list.append(TopPLogitsWarper(top_p))
     if top_k > 0:
         processor_list.append(TopKLogitsWarper(top_k))
     return processor_list
 
 
 class BatchingTask:
-    def __init__(self, tasks: List[GenerationTask], tokenizer: PreTrainedTokenizerBase, device: str, is_encoder_decoder: bool) -> None:
+    def __init__(self, tasks: List[GenerationTask], tokenizer: PreTrainedTokenizer, device: str, is_encoder_decoder: bool) -> None:
         self.batch_size = len(tasks)
         if self.batch_size == 0:
             return
         
         self.tokenizer = tokenizer
         self.device = device
         self.is_encoder_decoder = is_encoder_decoder
@@ -75,14 +82,16 @@
             logits_processor = prepare_logits_processor(
                 task.temperature, task.repetition_penalty, task.top_p, task.top_k
             )
             self.logits_processor_list.append(logits_processor)
         
         # variables used in the streaming process
         self.batch_tokens_cache: List[List[int]] = [[] for i in range(self.batch_size)]
+        self.batch_tokens_probs_cache: List[List[float]] = [[] for i in range(self.batch_size)]
+        self.batch_top_logprobs_cache: List[List[Dict[str, float]]] = [[] for i in range(self.batch_size)]
         self.stop = [False for i in range(self.batch_size)]
 
     def __len__(self):
         return self.batch_size
     
     def __call__(self, return_attention_mask=True) -> Any:
         ids = [torch.cat((self.prompts_ids[i], torch.LongTensor(self.batch_tokens_cache[i])))
@@ -128,35 +137,56 @@
     def get_prompt_length(self, idx:int) -> int:
         return len(self.get_prompt_ids(idx))
     
     def get_logits_processor_list(self, idx:int) -> LogitsProcessorList:
         self._check_idx(idx)
         return self.logits_processor_list[idx]
     
-    def get_generated_ids(self, idx:int) -> List[int]:
+    def get_generated_ids(self, idx: int) -> List[int]:
         self._check_idx(idx)
         return self.batch_tokens_cache[idx]
     
-    def get_generated_length(self, idx:int) -> int:
+    def get_generated_length(self, idx: int) -> int:
         return len(self.get_generated_ids(idx))
     
-    def update_new_token(self, batch_token: List[int]):
+    def get_generated_token_probs(self, idx: int) -> List[float]:
+        self._check_idx(idx)
+        return self.batch_tokens_probs_cache[idx]
+    
+    def get_generated_top_logprobs(self, idx: int) -> List[Dict[int, float]]:
+        self._check_idx(idx)
+        return self.batch_top_logprobs_cache[idx]
+    
+    def update_new_token(self, batch_token: List[int],
+            token_probs: Optional[List[Optional[float]]]=None,
+            top_logprobs: Optional[List[Optional[Dict[int, float]]]]=None
+        ):
         self._check_batch_size(batch_token)
+        if token_probs is not None:
+            self._check_batch_size(token_probs)
+        if top_logprobs is not None:
+            self._check_batch_size(top_logprobs)
+        
         for i, token in enumerate(batch_token):
             if self.is_stop(i):
                 continue
             self.batch_tokens_cache[i].append(token)
 
             # auto check stop
             if token == self.tokenizer.eos_token_id:
                 self.set_stop(i)
             if self.tasks[i].stop_token_ids is not None and token in self.tasks[i].stop_token_ids:
                 self.set_stop(i)
             if self.get_generated_length(i) == self.max_tokens[i]:
                 self.set_stop(i)
+            
+            if token_probs is not None and token_probs[i] is not None:
+                self.batch_tokens_probs_cache[i].append(token_probs[i])
+            if top_logprobs is not None and top_logprobs[i] is not None:
+                self.batch_top_logprobs_cache[i].append(top_logprobs[i])
                 
     def set_stop(self, idx:int):
         self._check_idx(idx)
         self.stop[idx] = True
     
     def is_stop(self, idx:int):
         self._check_idx(idx)
@@ -223,14 +253,17 @@
                     past_key_values=past_key_values,
                 )
             logits = out.logits
             past_key_values = out.past_key_values
             decoder_input_ids_list = []
 
             new_ids = []
+            # logprobs
+            token_probs = [None] * inputs.batch_size
+            top_logprobs = [None] * inputs.batch_size
 
             for i, task in enumerate(inputs.tasks):
                 if inputs.is_stop(i):
                     new_ids.append(inputs.pad_fill_id)
                     continue
                 each_logits = logits[i, -1, :].unsqueeze(0)
 
@@ -249,18 +282,26 @@
                     last_token_logits = last_token_logits.float().to("cpu")
 
                 if task.temperature < 1e-5 or task.top_p < 1e-8:  # greedy
                     token = int(torch.argmax(last_token_logits))
                 else:
                     probs = torch.softmax(last_token_logits, dim=-1)
                     token = int(torch.multinomial(probs, num_samples=1))
+                
+                if task.logprobs is not None:
+                    token_probs[i] = each_logits[0, token].item()
+                    top_values, top_indices = torch.topk(each_logits[0, :], task.logprobs, dim=-1, largest=True, sorted=True)
+                    item = {}
+                    for top_i in range(len(top_values)):
+                        item[top_indices[top_i].item()] = top_values[top_i].item()
+                    top_logprobs[i] = item
                 new_ids.append(token)
             
             # update state
-            inputs.update_new_token(new_ids)
+            inputs.update_new_token(new_ids, token_probs=token_probs, top_logprobs=top_logprobs)
             if streamer:
                 streamer.put(new_ids)
 
             if self.model.config.is_encoder_decoder or self.model.generation_config.use_cache:
                 # print("use cache!")
                 new_ids_tensor = torch.tensor(
                     new_ids, dtype=torch.long, device=decoder_input_ids.device).unsqueeze(1)
@@ -280,36 +321,97 @@
             streamer.end()
 
         del past_key_values
 
 class GenerationWorkerStreamer(BaseStreamer):
     def __init__(self,
                  task_batch: BatchingTask,
-                 tokenizer: PreTrainedTokenizerBase,
+                 tokenizer: PreTrainedTokenizer,
                  worker: "GenerationModelWorker") -> None:
         self.task_batch = task_batch
         self.tokenizer = tokenizer
         self.worker = worker
         self.stream_interval = worker.stream_interval
 
         self.done = [False for i in range(task_batch.batch_size)]
 
     def put(self, value):
         for i in range(self.task_batch.batch_size):
             generated_len = self.task_batch.get_generated_length(i)
             if (self.done[i] or generated_len % self.stream_interval != 0) and self.done[i]==self.task_batch.is_stop(i):
                 continue
             task = self.task_batch.tasks[i]
-            text = self.tokenizer.decode(self.task_batch.get_generated_ids(i), skip_special_tokens=True)
+
+            token_ids = self.task_batch.get_generated_ids(i)
+
+            # text = self.tokenizer.decode(token_ids, skip_special_tokens=True)
+            tokens = self.tokenizer.convert_ids_to_tokens(token_ids)
+            text = self.tokenizer.convert_tokens_to_string(tokens)
+
+            # get offset mapping from token to text
+            text_offset = []
+            for token_i in range(0, len(tokens)):
+                if token_i == 0:
+                    text_offset.append(-1)
+                    continue
+                prefix_text = self.tokenizer.convert_tokens_to_string(tokens[:token_i])
+                if text.startswith(prefix_text):
+                    text_offset.append(len(prefix_text))
+                else:
+                    text_offset.append(-1)
+            
+            last_id = len(text)
+            for token_i in reversed(range(0, len(tokens))):
+                if text_offset[token_i] == -1:
+                    text_offset[token_i] = last_id
+                else:
+                    last_id = text_offset[token_i]
+            
+            token_logprobs = self.task_batch.get_generated_token_probs(i)
+            top_logprobs = self.task_batch.get_generated_top_logprobs(i)
+            if top_logprobs is not None:
+                top_logprobs_new = []
+                for prob in top_logprobs:
+                    top_logprobs_new.append({self.tokenizer.convert_ids_to_tokens(k): v for k, v in prob.items()})
+                top_logprobs = top_logprobs_new
+
+            # remove stop words
             stop_pos = stop_by_stopwords(text, 0, task.stop)
             if stop_pos != -1:
+                token_stop_pos = len(tokens)
+                for token_i in reversed(range(0, len(text_offset))):
+                    if text_offset[token_i] < stop_pos:
+                        token_stop_pos = token_i + 1
+                        break
+    
                 self.task_batch.set_stop(i)
+
+                # remove tokens after stop pos
                 text = text[:stop_pos]
+                tokens = tokens[:token_stop_pos]
+                if token_logprobs is not None:
+                    token_logprobs = token_logprobs[:token_stop_pos]
+                if top_logprobs is not None:
+                    top_logprobs = top_logprobs[:token_stop_pos]
+                text_offset = text_offset[:token_stop_pos]
+            
             prompt_len = self.task_batch.get_prompt_length(i)
-
+            
+            # logprobs
+            if self.task_batch.tasks[i].logprobs is not None:
+                logprobs = GenerationWorkerLogprobs(
+                    tokens=tokens,
+                    token_logprobs=token_logprobs,
+                    top_logprobs=top_logprobs,
+                    text_offset=text_offset,
+                )
+            else:
+                logprobs = None
+            
+            # push task to queue
             if self.task_batch.is_stop(i):
                 if generated_len == self.task_batch.max_tokens[i]:
                     finish_reason = "length"
                 else:
                     finish_reason = "stop"
                 self.worker.push_task_result(task.task_id,
                     GenerationWorkerResult(
@@ -317,14 +419,15 @@
                         type="finish",
                         text=text,
                         usage=UsageInfo(
                             prompt_tokens=prompt_len,
                             total_tokens=prompt_len + generated_len,
                             completion_tokens=generated_len,
                         ),
+                        logprobs=logprobs,
                         finish_reason=finish_reason,
                     )
                 )
                 self.worker.push_task_result(task.task_id,
                     BaseWorkerResult(task_id=task.task_id, type="done")
                 )
                 self.done[i] = True
@@ -335,14 +438,15 @@
                         type="data",
                         text=text,
                         usage=UsageInfo(
                             prompt_tokens=prompt_len,
                             total_tokens=prompt_len + generated_len,
                             completion_tokens=generated_len,
                         ),
+                        logprobs=logprobs,
                         finish_reason=None,
                     )
                 )
 
     def end(self):
         # check all done
         self.put(None)
```

### Comparing `langport-0.3.0/langport/model/executor/generation/optimum.py` & `langport-0.3.1/langport/model/executor/generation/optimum.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/ggml.py` & `langport-0.3.1/langport/model/executor/ggml.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
         lib: Optional[str] = None,
         gpu_layers: int = 0,
         model_type: str = 'llama',
+        chunk_size: int = 1024,
+        threads: int = -1,
         load_8bit: bool = False,
         cpu_offloading: bool = False,
     ) -> None:
         super(GgmlExecutor, self).__init__(
             model_name = model_name,
             model_path = model_path,
             device = device,
@@ -40,21 +42,25 @@
             load_8bit = load_8bit,
             cpu_offloading = cpu_offloading,
         )
         self.gpu_layers = gpu_layers
         # ctransformers has a bug
         self.lib = lib
         self.model_type = model_type
+        self.chunk_size = chunk_size
+        self.threads = threads
  
 
     def load_model(self, model_path: str, from_pretrained_kwargs: dict):
         adapter = get_model_adapter(model_path)
         config = Config()
         setattr(config, 'stream', True)
         setattr(config, 'gpu_layers', self.gpu_layers)
+        setattr(config, 'batch_size', self.chunk_size)
+        setattr(config, 'threads', self.threads)
         auto_config = AutoConfig(config=config, model_type=self.model_type)
         model = AutoModelForCausalLM.from_pretrained(model_path,
                                                    config=auto_config,
                                                    lib=self.lib,
                                                    )
         tokenizer = GgmlTokenizer(model)
```

### Comparing `langport-0.3.0/langport/model/executor/huggingface.py` & `langport-0.3.1/langport/model/executor/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/executor/optimum.py` & `langport-0.3.1/langport/model/executor/optimum.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/model_adapter.py` & `langport-0.3.1/langport/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/model_args.py` & `langport-0.3.1/langport/model/model_args.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/models/rwkv_model.py` & `langport-0.3.1/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/model/monkey_patch_non_inplace.py` & `langport-0.3.1/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/protocol/huggingface_api_protocol.py` & `langport-0.3.1/langport/protocol/huggingface_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/protocol/openai_api_protocol.py` & `langport-0.3.1/langport/protocol/openai_api_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,18 +126,24 @@
     logprobs: Optional[int] = None
     echo: Optional[bool] = False
     presence_penalty: Optional[float] = 0.0
     frequency_penalty: Optional[float] = 0.0
     user: Optional[str] = None
 
 
+class CompletionLogprobs(BaseModel):
+    tokens: List[str]
+    token_logprobs: List[float]
+    top_logprobs: List[Dict[str, float]]
+    text_offset: List[int]
+
 class CompletionResponseChoice(BaseModel):
     index: int
     text: str
-    logprobs: Optional[int] = None
+    logprobs: Optional[CompletionLogprobs] = None
     finish_reason: Optional[Literal["stop", "length"]]
 
 
 class CompletionResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"cmpl-{shortuuid.random()}")
     object: str = "text_completion"
     created: int = Field(default_factory=lambda: int(time.time()))
@@ -145,15 +151,15 @@
     choices: List[CompletionResponseChoice]
     usage: UsageInfo
 
 
 class CompletionResponseStreamChoice(BaseModel):
     index: int
     text: str
-    logprobs: Optional[float] = None
+    logprobs: Optional[CompletionLogprobs] = None
     finish_reason: Optional[Literal["stop", "length"]] = None
 
 
 class CompletionStreamResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"cmpl-{shortuuid.random()}")
     object: str = "text_completion"
     created: int = Field(default_factory=lambda: int(time.time()))
```

### Comparing `langport-0.3.0/langport/protocol/tabby_api_protocol.py` & `langport-0.3.1/langport/protocol/tabby_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/protocol/worker_protocol.py` & `langport-0.3.1/langport/protocol/worker_protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     repetition_penalty: Optional[float] = 0.0
     top_p: Optional[float] = 1.0
     top_k: Optional[int] = 1
     max_tokens: Optional[int] = None
     stop: Optional[Union[List[str], str]] = None
     echo: Optional[bool] = False
     stop_token_ids: Optional[List[int]] = None
+    logprobs: Optional[int] = None
 
 class UsageInfo(BaseModel):
     prompt_tokens: int = 0
     total_tokens: int = 0
     completion_tokens: Optional[int] = 0
 
 class BaseWorkerResult(BaseModel):
@@ -102,12 +103,18 @@
     message: Optional[str] = None
     error_code: int = ErrorCode.OK
 
 class EmbeddingWorkerResult(BaseWorkerResult):
     embedding: List[float]
     usage: UsageInfo = None
 
+class GenerationWorkerLogprobs(BaseModel):
+    tokens: List[str]
+    token_logprobs: List[float]
+    top_logprobs: List[Dict[str, float]]
+    text_offset: List[int]
+
 class GenerationWorkerResult(BaseWorkerResult):
     text: str
-    logprobs: Optional[int] = None
+    logprobs: Optional[GenerationWorkerLogprobs] = None
     finish_reason: Optional[Literal["stop", "length"]] = None
     usage: UsageInfo = None
```

### Comparing `langport-0.3.0/langport/routers/gateway/common.py` & `langport-0.3.1/langport/routers/gateway/common.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/routers/gateway/openai_compatible.py` & `langport-0.3.1/langport/routers/gateway/openai_compatible.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from langport.protocol.openai_api_protocol import (
     ChatCompletionRequest,
     ChatCompletionResponse,
     ChatCompletionResponseStreamChoice,
     ChatCompletionStreamResponse,
     ChatMessage,
     ChatCompletionResponseChoice,
+    CompletionLogprobs,
     CompletionRequest,
     CompletionResponse,
     CompletionResponseChoice,
     DeltaMessage,
     CompletionResponseStreamChoice,
     CompletionStreamResponse,
     EmbeddingsData,
@@ -64,14 +65,15 @@
     *,
     temperature: float,
     top_p: float,
     max_tokens: Optional[int],
     echo: Optional[bool],
     stream: Optional[bool],
     stop: Optional[Union[str, List[str]]],
+    logprobs: Optional[int]=None,
 ) -> Dict[str, Any]:
     # is_chatglm = "chatglm" in model_name.lower()
     conv = get_conversation_template(model_name)
 
     if isinstance(messages, str):
         prompt = messages
     else:
@@ -97,14 +99,15 @@
         "model": model_name,
         "prompt": prompt,
         "temperature": temperature,
         "top_p": top_p,
         "max_tokens": max_tokens,
         "echo": echo,
         "stream": stream,
+        "logprobs": logprobs,
     }
 
     if stop is None:
         gen_params.update(
             {"stop": conv.settings.stop_str, "stop_token_ids": conv.settings.stop_token_ids}
         )
     else:
@@ -134,18 +137,22 @@
                 yield f"data: {json.dumps(content.dict(), ensure_ascii=False)}\n\n"
                 yield "data: [DONE]\n\n"
                 return
             decoded_unicode = content.text.replace("\ufffd", "")
             delta_text = decoded_unicode[len(previous_text) :]
             previous_text = decoded_unicode
 
+            if content.logprobs is None:
+                logprobs = None
+            else:
+                logprobs = CompletionLogprobs.parse_obj(content.logprobs.dict())
             choice_data = CompletionResponseStreamChoice(
                 index=i,
                 text=delta_text,
-                logprobs=content.logprobs,
+                logprobs=logprobs,
                 finish_reason=content.finish_reason,
             )
             chunk = CompletionStreamResponse(
                 id=id, object="text_completion", choices=[choice_data], model=model_name
             )
             if len(delta_text) == 0:
                 if content.finish_reason is not None:
@@ -301,19 +308,23 @@
 
     choices = []
     usage = UsageInfo()
     for i, content_task in enumerate(completions):
         content = await content_task
         if content.error_code != ErrorCode.OK:
             return create_error_response(content.error_code, content.message)
+        if content.logprobs is None:
+            logprobs = None
+        else:
+            logprobs = CompletionLogprobs.parse_obj(content.logprobs.dict())
         choices.append(
             CompletionResponseChoice(
                 index=i,
                 text=content.text,
-                logprobs=content.logprobs,
+                logprobs=logprobs,
                 finish_reason=content.finish_reason,
             )
         )
         task_usage = UsageInfo.parse_obj(content.usage)
         for usage_key, usage_value in task_usage.dict().items():
             setattr(usage, usage_key, getattr(usage, usage_key) + usage_value)
 
@@ -371,14 +382,15 @@
         request.prompt,
         temperature=request.temperature,
         top_p=request.top_p,
         max_tokens=request.max_tokens,
         echo=request.echo,
         stream=request.stream,
         stop=request.stop,
+        logprobs=request.logprobs,
     )
 
     if request.stream:
         return await completions_stream(app_settings, payload, request)
     else:
         return await completions_non_stream(app_settings, payload, request)
```

### Comparing `langport-0.3.0/langport/routers/server/core_node.py` & `langport-0.3.1/langport/routers/server/core_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/routers/server/embedding_node.py` & `langport-0.3.1/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/routers/server/generation_node.py` & `langport-0.3.1/langport/routers/server/generation_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         repetition_penalty=params.get("repetition_penalty", 0.0),
         top_p=params.get("top_p", 1.0),
         top_k=params.get("top_k", 1),
         max_tokens=params.get("max_tokens", 512),
         stop=params.get("stop", None),
         echo=params.get("echo", False),
         stop_token_ids=params.get("stop_token_ids", None),
+        logprobs=params.get("logprobs", None),
     ))
     background_tasks = create_background_tasks(app.node)
     return StreamingResponse(generator, background=background_tasks)
 
 
 @app.post("/completion")
 async def api_completion(request: Request):
@@ -75,13 +76,14 @@
         repetition_penalty=params.get("repetition_penalty", 0.0),
         top_p=params.get("top_p", 1.0),
         top_k=params.get("top_k", 1),
         max_tokens=params.get("max_tokens", 512),
         stop=params.get("stop", None),
         echo=params.get("echo", False),
         stop_token_ids=params.get("stop_token_ids", None),
+        logprobs=params.get("logprobs", None),
     ))
     completion = None
     for chunk in generator:
         completion = chunk
     background_tasks = create_background_tasks(app.node)
     return JSONResponse(content=completion.dict(), background=background_tasks)
```

### Comparing `langport-0.3.0/langport/service/gateway/cluster_monitor.py` & `langport-0.3.1/langport/service/gateway/cluster_monitor.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/gateway/cluster_monitor_app.py` & `langport-0.3.1/langport/service/gateway/cluster_monitor_app.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/gateway/fauxpilot_api.py` & `langport-0.3.1/langport/service/gateway/fauxpilot_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/gateway/graphite_feeder.py` & `langport-0.3.1/langport/service/gateway/graphite_feeder.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/gateway/huggingface_api.py` & `langport-0.3.1/langport/service/gateway/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/gateway/openai_api.py` & `langport-0.3.1/langport/service/gateway/openai_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/gateway/tabby_api.py` & `langport-0.3.1/langport/service/gateway/tabby_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/server/chatgpt_generation_worker.py` & `langport-0.3.1/langport/service/server/chatgpt_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/server/dummy_worker.py` & `langport-0.3.1/langport/service/server/dummy_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/server/embedding_worker.py` & `langport-0.3.1/langport/service/server/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/server/generation_worker.py` & `langport-0.3.1/langport/service/server/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/service/server/ggml_generation_worker.py` & `langport-0.3.1/langport/service/server/ggml_generation_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,18 @@
     parser.add_argument("--port", type=int, default=None)
     parser.add_argument("--worker-address", type=str, default=None)
     parser.add_argument("--neighbors", type=str, nargs="*", default=[])
 
     add_model_args(parser)
     parser.add_argument("--model-name", type=str, help="Optional display name")
     parser.add_argument("--limit-model-concurrency", type=int, default=8)
-    parser.add_argument("--batch", type=int, default=1)
     parser.add_argument("--stream-interval", type=int, default=2)
 
+    parser.add_argument("--chunk-size", type=int, default=512)
+    parser.add_argument("--threads", type=int, default=-1)
     parser.add_argument("--context-length", type=int, default=2048)
     parser.add_argument("--gpu-layers", type=int, default=0)
     parser.add_argument("--lib", type=str, default=None, choices=["avx2", "avx", "basic"], help="The path to a shared library or one of avx2, avx, basic.")
     parser.add_argument("--model-type", type=str, default="llama", choices=["llama", "gpt2", "dolly-v2", "starcoder"], help="The type of model to use.")
     args = parser.parse_args()
 
     node_id = str(uuid.uuid4())
@@ -54,20 +55,22 @@
     executor = GgmlGenerationExecutor(
         model_name=args.model_name,
         model_path=args.model_path,
         context_length=args.context_length,
         gpu_layers=args.gpu_layers,
         lib=args.lib,
         model_type=args.model_type,
+        chunk_size=args.chunk_size,
+        threads=args.threads,
     )
 
     app.node = GenerationModelWorker(
         node_addr=args.worker_address,
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         executor=executor,
         limit_model_concurrency=args.limit_model_concurrency,
-        max_batch=args.batch,
+        max_batch=1,
         stream_interval=args.stream_interval,
         logger=logger,
     )
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

### Comparing `langport-0.3.0/langport/service/server/optimum_generation_worker.py` & `langport-0.3.1/langport/service/server/optimum_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/utils/__init__.py` & `langport-0.3.1/langport/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/utils/evaluation.py` & `langport-0.3.1/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/utils/http_pool.py` & `langport-0.3.1/langport/utils/http_pool.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/utils/interval_timer.py` & `langport-0.3.1/langport/utils/interval_timer.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/workers/embedding_worker.py` & `langport-0.3.1/langport/workers/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.0/langport/workers/generation_worker.py` & `langport-0.3.1/langport/workers/generation_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 
     async def set_features(self):
         await self.set_local_state("features", ["generation"], ttl=360)
     
     async def set_model_name(self):
         await self.set_local_state("model_name", self.executor.model_name, ttl=360)
 
-
     async def generation_stream(self, task: GenerationTask):
         prompt_tokens = len(self.executor.tokenize(task.prompt))
         max_tokens = task.max_tokens
         context_length = self.executor.context_length
 
         if context_length is not None and prompt_tokens + max_tokens > context_length:
             yield BaseWorkerResult(task_id=task.task_id,
```

### Comparing `langport-0.3.0/langport.egg-info/PKG-INFO` & `langport-0.3.1/langport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.3.0
+Version: 0.3.1
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -67,14 +67,15 @@
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
 - [2023/05/22] New distributed architecture.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.3.0 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.3.1 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
 Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -20,41 +20,42 @@
 RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
 LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
 LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
 ## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
 V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
 server, and the following figure shows the Queries Per Second (QPS) and Tokens
 Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18]
-Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09]
-Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
-worker support. - [2023/06/01] Add HuggingFace text generation API support. -
-[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
-script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
-inference supported. - [2023/05/10] Langport project started. ## Install ###
-Method 1: With pip ```bash pip install langport ``` or: ```bash pip install
-git+https://github.com/vtuber-plan/langport.git ``` If you need ggml generation
-worker, use this command: ```bash pip install langport[ggml] ``` If you wanna
-use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From
-source 1. Clone this repository ```bash git clone https://github.com/vtuber-
-plan/langport.git cd langport ``` 2. Install the Package ```bash pip install --
-upgrade pip pip install -e . ``` ## Start the server It is simple to start a
-single node chat API service: ``` bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  python -
-m langport.service.gateway.openai_api ``` If you need the embeddings API or
-other features, you can deploy a distributed inference cluster: ``` bash python
--m langport.service.server.dummy_worker --port 21001 python -
-m langport.service.server.generation_worker --model-path  --neighbors http://
-localhost:21001 python -m langport.service.server.embedding_worker --model-path
---neighbors http://localhost:21001 python -
-m langport.service.gateway.openai_api --controller-address http://localhost:
-21001 ``` In practice, the gateway can connect to any node to distribute
-inference tasks: ``` bash python -m langport.service.server.dummy_worker --port
-21001 python -m langport.service.server.generation_worker --port 21002 --model-
-path  --neighbors http://localhost:21001 python -
+settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/07/13]
+Support generation logprobs parameter. - [2023/06/18] Add ggml (llama.cpp
+gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add LLama.cpp worker
+support. - [2023/06/01] Add HuggingFace Bert embedding worker support. - [2023/
+06/01] Add HuggingFace text generation API support. - [2023/06/01] Add tabby
+API support. - [2023/05/23] Add chat throughput test script. - [2023/05/22] New
+distributed architecture. - [2023/05/14] Batch inference supported. - [2023/05/
+10] Langport project started. ## Install ### Method 1: With pip ```bash pip
+install langport ``` or: ```bash pip install git+https://github.com/vtuber-
+plan/langport.git ``` If you need ggml generation worker, use this command:
+```bash pip install langport[ggml] ``` If you wanna use GPU: ```bash
+CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1. Clone
+this repository ```bash git clone https://github.com/vtuber-plan/langport.git
+cd langport ``` 2. Install the Package ```bash pip install --upgrade pip pip
+install -e . ``` ## Start the server It is simple to start a single node chat
+API service: ``` bash python -m langport.service.server.generation_worker --
+port 21001 --model-path  python -m langport.service.gateway.openai_api ``` If
+you need the embeddings API or other features, you can deploy a distributed
+inference cluster: ``` bash python -m langport.service.server.dummy_worker --
+port 21001 python -m langport.service.server.generation_worker --model-path  --
+neighbors http://localhost:21001 python -
+m langport.service.server.embedding_worker --model-path  --neighbors http://
+localhost:21001 python -m langport.service.gateway.openai_api --controller-
+address http://localhost:21001 ``` In practice, the gateway can connect to any
+node to distribute inference tasks: ``` bash python -
+m langport.service.server.dummy_worker --port 21001 python -
+m langport.service.server.generation_worker --port 21002 --model-path  --
+neighbors http://localhost:21001 python -
 m langport.service.server.generation_worker --port 21003 --model-path  --
 neighbors http://localhost:21001 http://localhost:21002 python -
 m langport.service.server.generation_worker --port 21004 --model-path  --
 neighbors http://localhost:21001 http://localhost:21003 python -
 m langport.service.server.generation_worker --port 21005 --model-path  --
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
```

### Comparing `langport-0.3.0/langport.egg-info/SOURCES.txt` & `langport-0.3.1/langport.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 langport/data/conversation/settings/chatgpt.py
 langport/data/conversation/settings/claude.py
 langport/data/conversation/settings/dolly.py
 langport/data/conversation/settings/falcon.py
 langport/data/conversation/settings/h2ogpt.py
 langport/data/conversation/settings/koala.py
 langport/data/conversation/settings/mpt.py
+langport/data/conversation/settings/ningyu.py
 langport/data/conversation/settings/oasst_pythia.py
 langport/data/conversation/settings/one_shot.py
 langport/data/conversation/settings/openbuddy.py
 langport/data/conversation/settings/phoenix.py
 langport/data/conversation/settings/redpajama.py
 langport/data/conversation/settings/rwkv.py
 langport/data/conversation/settings/stablelm.py
@@ -52,14 +53,15 @@
 langport/model/adapters/chatglm.py
 langport/model/adapters/chatgpt.py
 langport/model/adapters/claude.py
 langport/model/adapters/codegen.py
 langport/model/adapters/dolly_v2.py
 langport/model/adapters/falcon.py
 langport/model/adapters/koala.py
+langport/model/adapters/ningyu.py
 langport/model/adapters/oasst_pythia.py
 langport/model/adapters/openbuddy.py
 langport/model/adapters/phoenix.py
 langport/model/adapters/rwkv.py
 langport/model/adapters/stable_lm.py
 langport/model/adapters/starcoder.py
 langport/model/adapters/t5.py
```

### Comparing `langport-0.3.0/pyproject.toml` & `langport-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.3.0"
+version = "0.3.1"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

