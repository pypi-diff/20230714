# Comparing `tmp/xinference-0.0.3.tar.gz` & `tmp/xinference-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.0.3.tar", last modified: Tue Jul 11 13:52:52 2023, max compression
+gzip compressed data, was "xinference-0.0.4.tar", last modified: Fri Jul 14 12:15:56 2023, max compression
```

## Comparing `xinference-0.0.3.tar` & `xinference-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-11 13:52:44.000000 xinference-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 13:52:44.000000 xinference-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-11 13:52:52.991647 xinference-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-11 13:52:44.000000 xinference-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-11 13:52:44.000000 xinference-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 13:52:52.991647 xinference-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-11 13:52:44.000000 xinference-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-11 13:52:44.000000 xinference-0.0.3/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/locale/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/locale/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.991647 xinference-0.0.3/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/model/llm/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-11 13:52:44.000000 xinference-0.0.3/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:52:52.987647 xinference-0.0.3/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 13:52:52.000000 xinference-0.0.3/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-14 12:15:47.000000 xinference-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-14 12:15:47.000000 xinference-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-14 12:15:56.718407 xinference-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-14 12:15:47.000000 xinference-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 12:15:47.000000 xinference-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-14 12:15:56.718407 xinference-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-14 12:15:47.000000 xinference-0.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-14 12:15:47.000000 xinference-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.718407 xinference-0.0.4/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/model/llm/wizardlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-14 12:15:47.000000 xinference-0.0.4/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:15:56.714407 xinference-0.0.4/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 12:15:56.000000 xinference-0.0.4/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.0.3/LICENSE` & `xinference-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/PKG-INFO` & `xinference-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.3
+Version: 0.0.4
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -18,61 +18,59 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
+<div align="center">
+<img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
+
+# Xorbits Inference: Model Serving Made Easy 🤖
+
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
+</div>
+<br />
 
-# Xorbits Inference: Model Serving Made Easy 🤖
-
-Welcome to the Xorbits Inference GitHub repository!
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
-Currently, Xorbits Inference relies on [ggml](https://github.com/ggerganov/ggml) for model serving,
-which is specifically designed to enable large models and high performance on commodity hardware. 
-We are actively working on expanding Xorbits Inference's support to include additional runtimes, 
-including PyTorch and JAX, in the near future.
-
 ![demo](assets/demo.gif)
 
 <div align="center">
 <i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
 </div>
 
+
 ## Key Features
-🌟 **Model Serving Made Easy**: Inference simplifies the process of serving large language, speech 
+🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
 recognition, and multimodal models. You can set up and deploy your models
 for experimentation and production with a single command.
 
 ⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
 command. Inference provides access to state-of-the-art open-source models!
 
-🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources. Xorbits 
-Inference intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to maximize
-performance and accelerate your model inference tasks.
-
-⚙️ **Flexible API and Interfaces**: Xorbits Inference offers multiple interfaces for interacting
-with your models. You can utilize the RPC and RESTful API(compatible with OpenAI API) to integrate
-your models with existing systems or use the command-line interface (CLI) and the intuitive WebUI
+🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources with
+[ggml](https://github.com/ggerganov/ggml). Xorbits Inference intelligently utilizes heterogeneous
+hardware, including GPUs and CPUs, to accelerate your model inference tasks.
+
+⚙️ **Flexible API and Interfaces**: Offer multiple interfaces for interacting
+with your models, supporting RPC, RESTful API(compatible with OpenAI API), CLI and WebUI
 for seamless management and monitoring.
 
-🌐 **Distributed Deployment**: Xorbits Inference excels in distributed deployment scenarios, 
-allowing the seamless distribution of model inference across multiple devices or machines. It
-leverages distributed computing techniques to parallelize and scale the inference process.
+🌐 **Distributed Deployment**: Excel in distributed deployment scenarios, 
+allowing the seamless distribution of model inference across multiple devices or machines.
 
 🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
 with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
```

#### html2text {}

```diff
@@ -1,98 +1,91 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.3 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.0.4 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Software Development :: Libraries Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all License-
-File: LICENSE [![PyPI Latest Release](https://img.shields.io/pypi/v/
-xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/) [!
-[License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)]
-(https://github.com/xorbitsai/inference/blob/main/LICENSE) [![Build Status]
-(https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/
-python.yaml?branch=main&style=for-the-
-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
-xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
+File: LICENSE
+  [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
+  Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
+(https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
+l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
+  blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
+  workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
+  badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
+  xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
-t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
-(https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
-badge)](https://twitter.com/xorbitsio) # Xorbits Inference: Model Serving Made
-Easy ð¤ Welcome to the Xorbits Inference GitHub repository! Xorbits Inference
-(Xinference) is a powerful and versatile library designed to serve language,
-speech recognition, and multimodal models. With Xorbits Inference, you can
-effortlessly deploy and serve your or state-of-the-art built-in models using
-just a single command. Whether you are a researcher, developer, or data
-scientist, Xorbits Inference empowers you to unleash the full potential of
-cutting-edge AI models. Currently, Xorbits Inference relies on [ggml](https://
-github.com/ggerganov/ggml) for model serving, which is specifically designed to
-enable large models and high performance on commodity hardware. We are actively
-working on expanding Xorbits Inference's support to include additional
-runtimes, including PyTorch and JAX, in the near future. ![demo](assets/
-demo.gif)
+  t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
+ (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
+                    badge)](https://twitter.com/xorbitsio)
+
+Xorbits Inference(Xinference) is a powerful and versatile library designed to
+serve language, speech recognition, and multimodal models. With Xorbits
+Inference, you can effortlessly deploy and serve your or state-of-the-art
+built-in models using just a single command. Whether you are a researcher,
+developer, or data scientist, Xorbits Inference empowers you to unleash the
+full potential of cutting-edge AI models. ![demo](assets/demo.gif)
                         ð_Join_our_Slack_community!
-## Key Features ð **Model Serving Made Easy**: Inference simplifies the
-process of serving large language, speech recognition, and multimodal models.
-You can set up and deploy your models for experimentation and production with a
-single command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-
-edge built-in models using a single command. Inference provides access to
-state-of-the-art open-source models! ð¥ **Heterogeneous Hardware
-Utilization**: Make the most of your hardware resources. Xorbits Inference
-intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to
-maximize performance and accelerate your model inference tasks. âï¸
-**Flexible API and Interfaces**: Xorbits Inference offers multiple interfaces
-for interacting with your models. You can utilize the RPC and RESTful API
-(compatible with OpenAI API) to integrate your models with existing systems or
-use the command-line interface (CLI) and the intuitive WebUI for seamless
-management and monitoring. ð **Distributed Deployment**: Xorbits Inference
-excels in distributed deployment scenarios, allowing the seamless distribution
-of model inference across multiple devices or machines. It leverages
-distributed computing techniques to parallelize and scale the inference
-process. ð **Built-in Integration with Third-Party Libraries**: Xorbits
-Inference seamlessly integrates with popular third-party libraries like
-LangChain and LlamaIndex. (Coming soon) ## Getting Started Xinference can be
-installed via pip from PyPI. It is highly recommended to create a new virtual
-environment to avoid conflicts. ```bash $ pip install "xinference[all]" ```
-"xinference[all]" installs all the necessary packages for serving models. If
-you want to achieve acceleration on different hardware, refer to the
-installation documentation of the corresponding package. - [llama-cpp-python]
-(https://github.com/abetlen/llama-cpp-python#installation-from-pypi-
-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and
-`orca`. - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-
-started) is required to run `chatglm` and `chatglm2`. ### Deployment You can
-deploy Xinference locally with a single command or deploy it in a distributed
-cluster. #### Local To start a local instance of Xinference, run the following
-command: ```bash $ xinference ``` #### Distributed To deploy Xinference in a
-cluster, you need to start a Xinference supervisor on one server and Xinference
-workers on the other servers. Follow the steps below: **Starting the
-Supervisor**: On the server where you want to run the Xinference supervisor,
-run the following command: ```bash $ xinference-supervisor -H "$
-{supervisor_host}" ``` Replace `${supervisor_host}` with the actual host of
-your supervisor server. **Starting the Workers**: On each of the other servers
-where you want to run Xinference workers, run the following command: ```bash $
-xinference-worker -e "http://${supervisor_host}:9997" ``` Once Xinference is
-running, an endpoint will be accessible for model management via CLI or
-Xinference client. - For local deployment, the endpoint will be `http://
-localhost:9997`. - For cluster deployment, the endpoint will be `http://$
-{supervisor_host}:9997`, where `${supervisor_host}` is the hostname or IP
-address of the server where the supervisor is running. You can also view a web
-UI using the Xinference endpoint to chat with all the builtin models. You can
-even **chat with two cutting-edge AI models side-by-side to compare their
-performance**! ![web UI](assets/xinference-downloading.png) ### Xinference CLI
-Xinference provides a command line interface (CLI) for model management. Here
-are some useful commands: - Launch a model (a model UID will be returned):
-`xinference launch` - List running models: `xinference list` - List all the
-builtin models: `xinference list --all` - Terminate a model: `xinference
-terminate --model-uid ${model_uid}` ### Xinference Client Xinference also
-provides a client for managing and accessing models programmatically: ```python
-from xinference.client import Client client = Client("http://localhost:9997")
+## Key Features ð **Model Serving Made Easy**: Simplify the process of
+serving large language, speech recognition, and multimodal models. You can set
+up and deploy your models for experimentation and production with a single
+command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-edge
+built-in models using a single command. Inference provides access to state-of-
+the-art open-source models! ð¥ **Heterogeneous Hardware Utilization**: Make
+the most of your hardware resources with [ggml](https://github.com/ggerganov/
+ggml). Xorbits Inference intelligently utilizes heterogeneous hardware,
+including GPUs and CPUs, to accelerate your model inference tasks. âï¸
+**Flexible API and Interfaces**: Offer multiple interfaces for interacting with
+your models, supporting RPC, RESTful API(compatible with OpenAI API), CLI and
+WebUI for seamless management and monitoring. ð **Distributed Deployment**:
+Excel in distributed deployment scenarios, allowing the seamless distribution
+of model inference across multiple devices or machines. ð **Built-in
+Integration with Third-Party Libraries**: Xorbits Inference seamlessly
+integrates with popular third-party libraries like LangChain and LlamaIndex.
+(Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
+It is highly recommended to create a new virtual environment to avoid
+conflicts. ```bash $ pip install "xinference[all]" ``` "xinference[all]"
+installs all the necessary packages for serving models. If you want to achieve
+acceleration on different hardware, refer to the installation documentation of
+the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
+llama-cpp-python#installation-from-pypi-recommended) is required to run
+`baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
+(https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
+`chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
+a single command or deploy it in a distributed cluster. #### Local To start a
+local instance of Xinference, run the following command: ```bash $ xinference
+``` #### Distributed To deploy Xinference in a cluster, you need to start a
+Xinference supervisor on one server and Xinference workers on the other
+servers. Follow the steps below: **Starting the Supervisor**: On the server
+where you want to run the Xinference supervisor, run the following command:
+```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
+{supervisor_host}` with the actual host of your supervisor server. **Starting
+the Workers**: On each of the other servers where you want to run Xinference
+workers, run the following command: ```bash $ xinference-worker -e "http://$
+{supervisor_host}:9997" ``` Once Xinference is running, an endpoint will be
+accessible for model management via CLI or Xinference client. - For local
+deployment, the endpoint will be `http://localhost:9997`. - For cluster
+deployment, the endpoint will be `http://${supervisor_host}:9997`, where `$
+{supervisor_host}` is the hostname or IP address of the server where the
+supervisor is running. You can also view a web UI using the Xinference endpoint
+to chat with all the builtin models. You can even **chat with two cutting-edge
+AI models side-by-side to compare their performance**! ![web UI](assets/
+xinference-downloading.png) ### Xinference CLI Xinference provides a command
+line interface (CLI) for model management. Here are some useful commands: -
+Launch a model (a model UID will be returned): `xinference launch` - List
+running models: `xinference list` - List all the builtin models: `xinference
+list --all` - Terminate a model: `xinference terminate --model-uid $
+{model_uid}` ### Xinference Client Xinference also provides a client for
+managing and accessing models programmatically: ```python from
+xinference.client import Client client = Client("http://localhost:9997")
 model_uid = client.launch_model(model_name="chatglm2") model = client.get_model
 (model_uid) chat_history = [] prompt = "What is the largest animal?" model.chat
 ( prompt, chat_history, generate_config={"max_tokens": 1024} ) ``` Result:
 ```json { "id": "chatcmpl-8d76b65a-bad0-42ef-912d-4a0533d90d61", "model":
 "56f69622-1e73-11ee-a3bd-9af9f16816c6", "object": "chat.completion", "created":
 1688919187, "choices": [ { "index": 0, "message": { "role": "assistant",
 "content": "The largest animal that has been scientifically measured is the
```

### Comparing `xinference-0.0.3/README.md` & `xinference-0.0.4/xinference.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,76 @@
+Metadata-Version: 2.1
+Name: xinference
+Version: 0.0.4
+Summary: Model Serving Made Easy
+Home-page: https://github.com/xorbitsai/inference
+Author: Qin Xuye
+Author-email: qinxuye@xprobe.io
+Maintainer: Qin Xuye
+Maintainer-email: qinxuye@xprobe.io
+License: Apache License 2.0
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
+<div align="center">
+<img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
+
+# Xorbits Inference: Model Serving Made Easy 🤖
+
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
+</div>
+<br />
 
-# Xorbits Inference: Model Serving Made Easy 🤖
-
-Welcome to the Xorbits Inference GitHub repository!
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
-Currently, Xorbits Inference relies on [ggml](https://github.com/ggerganov/ggml) for model serving,
-which is specifically designed to enable large models and high performance on commodity hardware. 
-We are actively working on expanding Xorbits Inference's support to include additional runtimes, 
-including PyTorch and JAX, in the near future.
-
 ![demo](assets/demo.gif)
 
 <div align="center">
 <i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
 </div>
 
+
 ## Key Features
-🌟 **Model Serving Made Easy**: Inference simplifies the process of serving large language, speech 
+🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
 recognition, and multimodal models. You can set up and deploy your models
 for experimentation and production with a single command.
 
 ⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
 command. Inference provides access to state-of-the-art open-source models!
 
-🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources. Xorbits 
-Inference intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to maximize
-performance and accelerate your model inference tasks.
-
-⚙️ **Flexible API and Interfaces**: Xorbits Inference offers multiple interfaces for interacting
-with your models. You can utilize the RPC and RESTful API(compatible with OpenAI API) to integrate
-your models with existing systems or use the command-line interface (CLI) and the intuitive WebUI
+🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources with
+[ggml](https://github.com/ggerganov/ggml). Xorbits Inference intelligently utilizes heterogeneous
+hardware, including GPUs and CPUs, to accelerate your model inference tasks.
+
+⚙️ **Flexible API and Interfaces**: Offer multiple interfaces for interacting
+with your models, supporting RPC, RESTful API(compatible with OpenAI API), CLI and WebUI
 for seamless management and monitoring.
 
-🌐 **Distributed Deployment**: Xorbits Inference excels in distributed deployment scenarios, 
-allowing the seamless distribution of model inference across multiple devices or machines. It
-leverages distributed computing techniques to parallelize and scale the inference process.
+🌐 **Distributed Deployment**: Excel in distributed deployment scenarios, 
+allowing the seamless distribution of model inference across multiple devices or machines.
 
 🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
 with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
```

#### html2text {}

```diff
@@ -1,87 +1,91 @@
-[![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-
-the-badge)](https://pypi.org/project/xinference/) [![License](https://
-img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/
-xorbitsai/inference/blob/main/LICENSE) [![Build Status](https://img.shields.io/
-github/actions/workflow/status/xorbitsai/inference/
-python.yaml?branch=main&style=for-the-
-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
-xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
+Metadata-Version: 2.1 Name: xinference Version: 0.0.4 Summary: Model Serving
+Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
+Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
+qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Software Development :: Libraries Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all License-
+File: LICENSE
+  [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
+  Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
+(https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
+l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
+  blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
+  workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
+  badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
+  xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
-t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
-(https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
-badge)](https://twitter.com/xorbitsio) # Xorbits Inference: Model Serving Made
-Easy ð¤ Welcome to the Xorbits Inference GitHub repository! Xorbits Inference
-(Xinference) is a powerful and versatile library designed to serve language,
-speech recognition, and multimodal models. With Xorbits Inference, you can
-effortlessly deploy and serve your or state-of-the-art built-in models using
-just a single command. Whether you are a researcher, developer, or data
-scientist, Xorbits Inference empowers you to unleash the full potential of
-cutting-edge AI models. Currently, Xorbits Inference relies on [ggml](https://
-github.com/ggerganov/ggml) for model serving, which is specifically designed to
-enable large models and high performance on commodity hardware. We are actively
-working on expanding Xorbits Inference's support to include additional
-runtimes, including PyTorch and JAX, in the near future. ![demo](assets/
-demo.gif)
+  t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
+ (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
+                    badge)](https://twitter.com/xorbitsio)
+
+Xorbits Inference(Xinference) is a powerful and versatile library designed to
+serve language, speech recognition, and multimodal models. With Xorbits
+Inference, you can effortlessly deploy and serve your or state-of-the-art
+built-in models using just a single command. Whether you are a researcher,
+developer, or data scientist, Xorbits Inference empowers you to unleash the
+full potential of cutting-edge AI models. ![demo](assets/demo.gif)
                         ð_Join_our_Slack_community!
-## Key Features ð **Model Serving Made Easy**: Inference simplifies the
-process of serving large language, speech recognition, and multimodal models.
-You can set up and deploy your models for experimentation and production with a
-single command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-
-edge built-in models using a single command. Inference provides access to
-state-of-the-art open-source models! ð¥ **Heterogeneous Hardware
-Utilization**: Make the most of your hardware resources. Xorbits Inference
-intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to
-maximize performance and accelerate your model inference tasks. âï¸
-**Flexible API and Interfaces**: Xorbits Inference offers multiple interfaces
-for interacting with your models. You can utilize the RPC and RESTful API
-(compatible with OpenAI API) to integrate your models with existing systems or
-use the command-line interface (CLI) and the intuitive WebUI for seamless
-management and monitoring. ð **Distributed Deployment**: Xorbits Inference
-excels in distributed deployment scenarios, allowing the seamless distribution
-of model inference across multiple devices or machines. It leverages
-distributed computing techniques to parallelize and scale the inference
-process. ð **Built-in Integration with Third-Party Libraries**: Xorbits
-Inference seamlessly integrates with popular third-party libraries like
-LangChain and LlamaIndex. (Coming soon) ## Getting Started Xinference can be
-installed via pip from PyPI. It is highly recommended to create a new virtual
-environment to avoid conflicts. ```bash $ pip install "xinference[all]" ```
-"xinference[all]" installs all the necessary packages for serving models. If
-you want to achieve acceleration on different hardware, refer to the
-installation documentation of the corresponding package. - [llama-cpp-python]
-(https://github.com/abetlen/llama-cpp-python#installation-from-pypi-
-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and
-`orca`. - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-
-started) is required to run `chatglm` and `chatglm2`. ### Deployment You can
-deploy Xinference locally with a single command or deploy it in a distributed
-cluster. #### Local To start a local instance of Xinference, run the following
-command: ```bash $ xinference ``` #### Distributed To deploy Xinference in a
-cluster, you need to start a Xinference supervisor on one server and Xinference
-workers on the other servers. Follow the steps below: **Starting the
-Supervisor**: On the server where you want to run the Xinference supervisor,
-run the following command: ```bash $ xinference-supervisor -H "$
-{supervisor_host}" ``` Replace `${supervisor_host}` with the actual host of
-your supervisor server. **Starting the Workers**: On each of the other servers
-where you want to run Xinference workers, run the following command: ```bash $
-xinference-worker -e "http://${supervisor_host}:9997" ``` Once Xinference is
-running, an endpoint will be accessible for model management via CLI or
-Xinference client. - For local deployment, the endpoint will be `http://
-localhost:9997`. - For cluster deployment, the endpoint will be `http://$
-{supervisor_host}:9997`, where `${supervisor_host}` is the hostname or IP
-address of the server where the supervisor is running. You can also view a web
-UI using the Xinference endpoint to chat with all the builtin models. You can
-even **chat with two cutting-edge AI models side-by-side to compare their
-performance**! ![web UI](assets/xinference-downloading.png) ### Xinference CLI
-Xinference provides a command line interface (CLI) for model management. Here
-are some useful commands: - Launch a model (a model UID will be returned):
-`xinference launch` - List running models: `xinference list` - List all the
-builtin models: `xinference list --all` - Terminate a model: `xinference
-terminate --model-uid ${model_uid}` ### Xinference Client Xinference also
-provides a client for managing and accessing models programmatically: ```python
-from xinference.client import Client client = Client("http://localhost:9997")
+## Key Features ð **Model Serving Made Easy**: Simplify the process of
+serving large language, speech recognition, and multimodal models. You can set
+up and deploy your models for experimentation and production with a single
+command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-edge
+built-in models using a single command. Inference provides access to state-of-
+the-art open-source models! ð¥ **Heterogeneous Hardware Utilization**: Make
+the most of your hardware resources with [ggml](https://github.com/ggerganov/
+ggml). Xorbits Inference intelligently utilizes heterogeneous hardware,
+including GPUs and CPUs, to accelerate your model inference tasks. âï¸
+**Flexible API and Interfaces**: Offer multiple interfaces for interacting with
+your models, supporting RPC, RESTful API(compatible with OpenAI API), CLI and
+WebUI for seamless management and monitoring. ð **Distributed Deployment**:
+Excel in distributed deployment scenarios, allowing the seamless distribution
+of model inference across multiple devices or machines. ð **Built-in
+Integration with Third-Party Libraries**: Xorbits Inference seamlessly
+integrates with popular third-party libraries like LangChain and LlamaIndex.
+(Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
+It is highly recommended to create a new virtual environment to avoid
+conflicts. ```bash $ pip install "xinference[all]" ``` "xinference[all]"
+installs all the necessary packages for serving models. If you want to achieve
+acceleration on different hardware, refer to the installation documentation of
+the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
+llama-cpp-python#installation-from-pypi-recommended) is required to run
+`baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
+(https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
+`chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
+a single command or deploy it in a distributed cluster. #### Local To start a
+local instance of Xinference, run the following command: ```bash $ xinference
+``` #### Distributed To deploy Xinference in a cluster, you need to start a
+Xinference supervisor on one server and Xinference workers on the other
+servers. Follow the steps below: **Starting the Supervisor**: On the server
+where you want to run the Xinference supervisor, run the following command:
+```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
+{supervisor_host}` with the actual host of your supervisor server. **Starting
+the Workers**: On each of the other servers where you want to run Xinference
+workers, run the following command: ```bash $ xinference-worker -e "http://$
+{supervisor_host}:9997" ``` Once Xinference is running, an endpoint will be
+accessible for model management via CLI or Xinference client. - For local
+deployment, the endpoint will be `http://localhost:9997`. - For cluster
+deployment, the endpoint will be `http://${supervisor_host}:9997`, where `$
+{supervisor_host}` is the hostname or IP address of the server where the
+supervisor is running. You can also view a web UI using the Xinference endpoint
+to chat with all the builtin models. You can even **chat with two cutting-edge
+AI models side-by-side to compare their performance**! ![web UI](assets/
+xinference-downloading.png) ### Xinference CLI Xinference provides a command
+line interface (CLI) for model management. Here are some useful commands: -
+Launch a model (a model UID will be returned): `xinference launch` - List
+running models: `xinference list` - List all the builtin models: `xinference
+list --all` - Terminate a model: `xinference terminate --model-uid $
+{model_uid}` ### Xinference Client Xinference also provides a client for
+managing and accessing models programmatically: ```python from
+xinference.client import Client client = Client("http://localhost:9997")
 model_uid = client.launch_model(model_name="chatglm2") model = client.get_model
 (model_uid) chat_history = [] prompt = "What is the largest animal?" model.chat
 ( prompt, chat_history, generate_config={"max_tokens": 1024} ) ``` Result:
 ```json { "id": "chatcmpl-8d76b65a-bad0-42ef-912d-4a0533d90d61", "model":
 "56f69622-1e73-11ee-a3bd-9af9f16816c6", "object": "chat.completion", "created":
 1688919187, "choices": [ { "index": 0, "message": { "role": "assistant",
 "content": "The largest animal that has been scientifically measured is the
```

### Comparing `xinference-0.0.3/setup.cfg` & `xinference-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/setup.py` & `xinference-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/versioneer.py` & `xinference-0.0.4/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/__init__.py` & `xinference-0.0.4/xinference/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/constants.py` & `xinference-0.0.4/xinference/constants.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/core/__init__.py` & `xinference-0.0.4/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/core/api.py` & `xinference-0.0.4/xinference/core/api.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/core/gradio.py` & `xinference-0.0.4/xinference/core/gradio.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/core/model.py` & `xinference-0.0.4/xinference/core/model.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/core/resource.py` & `xinference-0.0.4/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/core/restful_api.py` & `xinference-0.0.4/xinference/core/restful_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from ..types import ChatCompletion, Completion
 from .service import SupervisorActor
 
 logger = logging.getLogger(__name__)
 
 max_tokens_field = Field(
-    default=16, ge=1, le=2048, description="The maximum number of tokens to generate."
+    default=128, ge=1, le=2048, description="The maximum number of tokens to generate."
 )
 
 temperature_field = Field(
     default=0.8,
     ge=0.0,
     le=2.0,
     description="Adjust the randomness of the generated text.\n\n"
@@ -232,14 +232,17 @@
             allow_origins=["*"],
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
         )
         self._router = APIRouter()
         self._router.add_api_route("/v1/models", self.list_models, methods=["GET"])
+        self._router.add_api_route(
+            "/v1/models/{model_uid}", self.describe_model, methods=["GET"]
+        )
         self._router.add_api_route("/v1/models", self.launch_model, methods=["POST"])
         self._router.add_api_route(
             "/v1/models/{model_uid}", self.terminate_model, methods=["DELETE"]
         )
         self._router.add_api_route("/v1/address", self.get_address, methods=["GET"])
         self._router.add_api_route(
             "/v1/completions",
@@ -284,14 +287,21 @@
                 "model_name": model_spec.model_name,
                 "model_format": model_spec.model_format,
                 "model_size_in_billions": model_spec.model_size_in_billions,
                 "quantization": model_spec.quantization,
             }
         return models_dict
 
+    async def describe_model(self, model_uid: str):
+        try:
+            return await self._supervisor_ref.describe_model(model_uid)
+        except Exception as e:
+            logger.error(e, exc_info=True)
+            raise HTTPException(status_code=500, detail=str(e))
+
     async def launch_model(self, request: Request) -> JSONResponse:
         payload = await request.json()
         model_uid = payload.get("model_uid")
         model_name = payload.get("model_name")
         model_size_in_billions = payload.get("model_size_in_billions")
         model_format = payload.get("model_format")
         quantization = payload.get("quantization")
```

### Comparing `xinference-0.0.3/xinference/core/service.py` & `xinference-0.0.4/xinference/core/service.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/__init__.py` & `xinference-0.0.4/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/cmdline.py` & `xinference-0.0.4/xinference/deploy/cmdline.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/local.py` & `xinference-0.0.4/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/supervisor.py` & `xinference-0.0.4/xinference/deploy/supervisor.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/test/__init__.py` & `xinference-0.0.4/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/utils.py` & `xinference-0.0.4/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/deploy/worker.py` & `xinference-0.0.4/xinference/deploy/worker.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/isolation.py` & `xinference-0.0.4/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/locale/__init__.py` & `xinference-0.0.4/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/locale/utils.py` & `xinference-0.0.4/xinference/locale/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/locale/zh_CN.json` & `xinference-0.0.4/xinference/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/model/__init__.py` & `xinference-0.0.4/xinference/model/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/model/llm/__init__.py` & `xinference-0.0.4/xinference/model/llm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,44 @@
                 "q8_0",
             ],
             url_generator=wizardlm_v1_0_url_generator,
             cls=WizardlmGgml,
         ),
     )
 
+    wizardlm_v1_1_url_generator = lambda model_size, quantization: (
+        f"https://huggingface.co/TheBloke/WizardLM-{model_size}B-V1.1-GGML/resolve/main/"
+        f"wizardlm-{model_size}b-v1.1.ggmlv3.{quantization}.bin"
+    )
+    MODEL_FAMILIES.append(
+        ModelFamily(
+            model_name="wizardlm-v1.1",
+            model_sizes_in_billions=[13],
+            model_format="ggmlv3",
+            quantizations=[
+                "q2_K",
+                "q3_K_L",
+                "q3_K_M",
+                "q3_K_S",
+                "q4_0",
+                "q4_1",
+                "q4_K_M",
+                "q4_K_S",
+                "q5_0",
+                "q5_1",
+                "q5_K_M",
+                "q5_K_S",
+                "q6_K",
+                "q8_0",
+            ],
+            url_generator=wizardlm_v1_1_url_generator,
+            cls=VicunaCensoredGgml,  # according to https://huggingface.co/TheBloke/WizardLM-13B-V1.1-GGML
+        ),
+    )
+
     vicuna_v1_3_url_generator = lambda model_size, quantization: (
         "https://huggingface.co/TheBloke/vicuna-7B-v1.3-GGML/resolve/main/"
         f"vicuna-7b-v1.3.ggmlv3.{quantization}.bin"
         if model_size == 7
         else (
             "https://huggingface.co/TheBloke/vicuna-13b-v1.3.0-GGML/resolve/main/"
             f"vicuna-13b-v1.3.0.ggmlv3.{quantization}.bin"
```

### Comparing `xinference-0.0.3/xinference/model/llm/chatglm.py` & `xinference-0.0.4/xinference/model/llm/chatglm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/model/llm/core.py` & `xinference-0.0.4/xinference/model/llm/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,26 +126,46 @@
         self._gpu_layers = SIZE_TO_GPU_LAYERS[closest_size]
         self._model_path = model_path
         self._llamacpp_model_config: LlamaCppModelConfig = self._sanitize_model_config(
             llamacpp_model_config
         )
         self._llm = None
 
+    @staticmethod
+    def _is_darwin_and_apple_silicon():
+        return platform.system() == "Darwin" and platform.processor() == "arm"
+
+    @staticmethod
+    def _is_linux():
+        return platform.system() == "Linux"
+
+    def _can_apply_metal(self):
+        return (
+            self.model_spec.quantization == "q4_0"
+            or self.model_spec.quantization == "q4_1"
+        )
+
+    def _can_apply_cublas(self):
+        # TODO: figure out the quantizations supported.
+        return True
+
     def _sanitize_model_config(
         self, llamacpp_model_config: Optional[LlamaCppModelConfig]
     ) -> LlamaCppModelConfig:
         if llamacpp_model_config is None:
             llamacpp_model_config = LlamaCppModelConfig()
         if platform.system() == "Windows":
-            context_length = 512
+            llamacpp_model_config.setdefault("n_ctx", 512)
         else:
-            context_length = 2048
+            llamacpp_model_config.setdefault("n_ctx", 2048)
 
-        llamacpp_model_config.setdefault("n_gpu_layers", self._gpu_layers)
-        llamacpp_model_config.setdefault("n_ctx", context_length)
+        if self._is_darwin_and_apple_silicon() and self._can_apply_metal():
+            llamacpp_model_config.setdefault("n_gpu_layers", 1)
+        elif self._is_linux() and self._can_apply_cublas():
+            llamacpp_model_config.setdefault("n_gpu_layers", self._gpu_layers)
 
         return llamacpp_model_config
 
     def _sanitize_generate_config(
         self, generate_config: Optional[LlamaCppGenerateConfig]
     ) -> LlamaCppGenerateConfig:
         if generate_config is None:
```

### Comparing `xinference-0.0.3/xinference/model/llm/orca.py` & `xinference-0.0.4/xinference/model/llm/orca.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/model/llm/vicuna.py` & `xinference-0.0.4/xinference/model/llm/vicuna.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/model/llm/wizardlm.py` & `xinference-0.0.4/xinference/model/llm/wizardlm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference/types.py` & `xinference-0.0.4/xinference/types.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.3/xinference.egg-info/PKG-INFO` & `xinference-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,52 @@
-Metadata-Version: 2.1
-Name: xinference
-Version: 0.0.3
-Summary: Model Serving Made Easy
-Home-page: https://github.com/xorbitsai/inference
-Author: Qin Xuye
-Author-email: qinxuye@xprobe.io
-Maintainer: Qin Xuye
-Maintainer-email: qinxuye@xprobe.io
-License: Apache License 2.0
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
+<div align="center">
+<img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
+
+# Xorbits Inference: Model Serving Made Easy 🤖
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
 [![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
+</div>
+<br />
 
-# Xorbits Inference: Model Serving Made Easy 🤖
-
-Welcome to the Xorbits Inference GitHub repository!
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
-Currently, Xorbits Inference relies on [ggml](https://github.com/ggerganov/ggml) for model serving,
-which is specifically designed to enable large models and high performance on commodity hardware. 
-We are actively working on expanding Xorbits Inference's support to include additional runtimes, 
-including PyTorch and JAX, in the near future.
-
 ![demo](assets/demo.gif)
 
 <div align="center">
 <i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
 </div>
 
+
 ## Key Features
-🌟 **Model Serving Made Easy**: Inference simplifies the process of serving large language, speech 
+🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
 recognition, and multimodal models. You can set up and deploy your models
 for experimentation and production with a single command.
 
 ⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
 command. Inference provides access to state-of-the-art open-source models!
 
-🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources. Xorbits 
-Inference intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to maximize
-performance and accelerate your model inference tasks.
-
-⚙️ **Flexible API and Interfaces**: Xorbits Inference offers multiple interfaces for interacting
-with your models. You can utilize the RPC and RESTful API(compatible with OpenAI API) to integrate
-your models with existing systems or use the command-line interface (CLI) and the intuitive WebUI
+🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources with
+[ggml](https://github.com/ggerganov/ggml). Xorbits Inference intelligently utilizes heterogeneous
+hardware, including GPUs and CPUs, to accelerate your model inference tasks.
+
+⚙️ **Flexible API and Interfaces**: Offer multiple interfaces for interacting
+with your models, supporting RPC, RESTful API(compatible with OpenAI API), CLI and WebUI
 for seamless management and monitoring.
 
-🌐 **Distributed Deployment**: Xorbits Inference excels in distributed deployment scenarios, 
-allowing the seamless distribution of model inference across multiple devices or machines. It
-leverages distributed computing techniques to parallelize and scale the inference process.
+🌐 **Distributed Deployment**: Excel in distributed deployment scenarios, 
+allowing the seamless distribution of model inference across multiple devices or machines.
 
 🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
 with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
```

#### html2text {}

```diff
@@ -1,98 +1,79 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.3 Summary: Model Serving
-Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
-Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
-qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Software Development :: Libraries Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all License-
-File: LICENSE [![PyPI Latest Release](https://img.shields.io/pypi/v/
-xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/) [!
-[License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)]
-(https://github.com/xorbitsai/inference/blob/main/LICENSE) [![Build Status]
-(https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/
-python.yaml?branch=main&style=for-the-
-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
-xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
+  [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
+  Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
+(https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
+l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
+  blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
+  workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
+  badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
+  xorbitsai/inference/goto?ref=main) [![Slack](https://img.shields.io/badge/
 join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/
-t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
-(https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
-badge)](https://twitter.com/xorbitsio) # Xorbits Inference: Model Serving Made
-Easy ð¤ Welcome to the Xorbits Inference GitHub repository! Xorbits Inference
-(Xinference) is a powerful and versatile library designed to serve language,
-speech recognition, and multimodal models. With Xorbits Inference, you can
-effortlessly deploy and serve your or state-of-the-art built-in models using
-just a single command. Whether you are a researcher, developer, or data
-scientist, Xorbits Inference empowers you to unleash the full potential of
-cutting-edge AI models. Currently, Xorbits Inference relies on [ggml](https://
-github.com/ggerganov/ggml) for model serving, which is specifically designed to
-enable large models and high performance on commodity hardware. We are actively
-working on expanding Xorbits Inference's support to include additional
-runtimes, including PyTorch and JAX, in the near future. ![demo](assets/
-demo.gif)
+  t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg) [![Twitter]
+ (https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-
+                    badge)](https://twitter.com/xorbitsio)
+
+Xorbits Inference(Xinference) is a powerful and versatile library designed to
+serve language, speech recognition, and multimodal models. With Xorbits
+Inference, you can effortlessly deploy and serve your or state-of-the-art
+built-in models using just a single command. Whether you are a researcher,
+developer, or data scientist, Xorbits Inference empowers you to unleash the
+full potential of cutting-edge AI models. ![demo](assets/demo.gif)
                         ð_Join_our_Slack_community!
-## Key Features ð **Model Serving Made Easy**: Inference simplifies the
-process of serving large language, speech recognition, and multimodal models.
-You can set up and deploy your models for experimentation and production with a
-single command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-
-edge built-in models using a single command. Inference provides access to
-state-of-the-art open-source models! ð¥ **Heterogeneous Hardware
-Utilization**: Make the most of your hardware resources. Xorbits Inference
-intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to
-maximize performance and accelerate your model inference tasks. âï¸
-**Flexible API and Interfaces**: Xorbits Inference offers multiple interfaces
-for interacting with your models. You can utilize the RPC and RESTful API
-(compatible with OpenAI API) to integrate your models with existing systems or
-use the command-line interface (CLI) and the intuitive WebUI for seamless
-management and monitoring. ð **Distributed Deployment**: Xorbits Inference
-excels in distributed deployment scenarios, allowing the seamless distribution
-of model inference across multiple devices or machines. It leverages
-distributed computing techniques to parallelize and scale the inference
-process. ð **Built-in Integration with Third-Party Libraries**: Xorbits
-Inference seamlessly integrates with popular third-party libraries like
-LangChain and LlamaIndex. (Coming soon) ## Getting Started Xinference can be
-installed via pip from PyPI. It is highly recommended to create a new virtual
-environment to avoid conflicts. ```bash $ pip install "xinference[all]" ```
-"xinference[all]" installs all the necessary packages for serving models. If
-you want to achieve acceleration on different hardware, refer to the
-installation documentation of the corresponding package. - [llama-cpp-python]
-(https://github.com/abetlen/llama-cpp-python#installation-from-pypi-
-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and
-`orca`. - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-
-started) is required to run `chatglm` and `chatglm2`. ### Deployment You can
-deploy Xinference locally with a single command or deploy it in a distributed
-cluster. #### Local To start a local instance of Xinference, run the following
-command: ```bash $ xinference ``` #### Distributed To deploy Xinference in a
-cluster, you need to start a Xinference supervisor on one server and Xinference
-workers on the other servers. Follow the steps below: **Starting the
-Supervisor**: On the server where you want to run the Xinference supervisor,
-run the following command: ```bash $ xinference-supervisor -H "$
-{supervisor_host}" ``` Replace `${supervisor_host}` with the actual host of
-your supervisor server. **Starting the Workers**: On each of the other servers
-where you want to run Xinference workers, run the following command: ```bash $
-xinference-worker -e "http://${supervisor_host}:9997" ``` Once Xinference is
-running, an endpoint will be accessible for model management via CLI or
-Xinference client. - For local deployment, the endpoint will be `http://
-localhost:9997`. - For cluster deployment, the endpoint will be `http://$
-{supervisor_host}:9997`, where `${supervisor_host}` is the hostname or IP
-address of the server where the supervisor is running. You can also view a web
-UI using the Xinference endpoint to chat with all the builtin models. You can
-even **chat with two cutting-edge AI models side-by-side to compare their
-performance**! ![web UI](assets/xinference-downloading.png) ### Xinference CLI
-Xinference provides a command line interface (CLI) for model management. Here
-are some useful commands: - Launch a model (a model UID will be returned):
-`xinference launch` - List running models: `xinference list` - List all the
-builtin models: `xinference list --all` - Terminate a model: `xinference
-terminate --model-uid ${model_uid}` ### Xinference Client Xinference also
-provides a client for managing and accessing models programmatically: ```python
-from xinference.client import Client client = Client("http://localhost:9997")
+## Key Features ð **Model Serving Made Easy**: Simplify the process of
+serving large language, speech recognition, and multimodal models. You can set
+up and deploy your models for experimentation and production with a single
+command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-edge
+built-in models using a single command. Inference provides access to state-of-
+the-art open-source models! ð¥ **Heterogeneous Hardware Utilization**: Make
+the most of your hardware resources with [ggml](https://github.com/ggerganov/
+ggml). Xorbits Inference intelligently utilizes heterogeneous hardware,
+including GPUs and CPUs, to accelerate your model inference tasks. âï¸
+**Flexible API and Interfaces**: Offer multiple interfaces for interacting with
+your models, supporting RPC, RESTful API(compatible with OpenAI API), CLI and
+WebUI for seamless management and monitoring. ð **Distributed Deployment**:
+Excel in distributed deployment scenarios, allowing the seamless distribution
+of model inference across multiple devices or machines. ð **Built-in
+Integration with Third-Party Libraries**: Xorbits Inference seamlessly
+integrates with popular third-party libraries like LangChain and LlamaIndex.
+(Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
+It is highly recommended to create a new virtual environment to avoid
+conflicts. ```bash $ pip install "xinference[all]" ``` "xinference[all]"
+installs all the necessary packages for serving models. If you want to achieve
+acceleration on different hardware, refer to the installation documentation of
+the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
+llama-cpp-python#installation-from-pypi-recommended) is required to run
+`baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
+(https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
+`chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
+a single command or deploy it in a distributed cluster. #### Local To start a
+local instance of Xinference, run the following command: ```bash $ xinference
+``` #### Distributed To deploy Xinference in a cluster, you need to start a
+Xinference supervisor on one server and Xinference workers on the other
+servers. Follow the steps below: **Starting the Supervisor**: On the server
+where you want to run the Xinference supervisor, run the following command:
+```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
+{supervisor_host}` with the actual host of your supervisor server. **Starting
+the Workers**: On each of the other servers where you want to run Xinference
+workers, run the following command: ```bash $ xinference-worker -e "http://$
+{supervisor_host}:9997" ``` Once Xinference is running, an endpoint will be
+accessible for model management via CLI or Xinference client. - For local
+deployment, the endpoint will be `http://localhost:9997`. - For cluster
+deployment, the endpoint will be `http://${supervisor_host}:9997`, where `$
+{supervisor_host}` is the hostname or IP address of the server where the
+supervisor is running. You can also view a web UI using the Xinference endpoint
+to chat with all the builtin models. You can even **chat with two cutting-edge
+AI models side-by-side to compare their performance**! ![web UI](assets/
+xinference-downloading.png) ### Xinference CLI Xinference provides a command
+line interface (CLI) for model management. Here are some useful commands: -
+Launch a model (a model UID will be returned): `xinference launch` - List
+running models: `xinference list` - List all the builtin models: `xinference
+list --all` - Terminate a model: `xinference terminate --model-uid $
+{model_uid}` ### Xinference Client Xinference also provides a client for
+managing and accessing models programmatically: ```python from
+xinference.client import Client client = Client("http://localhost:9997")
 model_uid = client.launch_model(model_name="chatglm2") model = client.get_model
 (model_uid) chat_history = [] prompt = "What is the largest animal?" model.chat
 ( prompt, chat_history, generate_config={"max_tokens": 1024} ) ``` Result:
 ```json { "id": "chatcmpl-8d76b65a-bad0-42ef-912d-4a0533d90d61", "model":
 "56f69622-1e73-11ee-a3bd-9af9f16816c6", "object": "chat.completion", "created":
 1688919187, "choices": [ { "index": 0, "message": { "role": "assistant",
 "content": "The largest animal that has been scientifically measured is the
```

### Comparing `xinference-0.0.3/xinference.egg-info/SOURCES.txt` & `xinference-0.0.4/xinference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

