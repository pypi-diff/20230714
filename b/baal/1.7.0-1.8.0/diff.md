# Comparing `tmp/baal-1.7.0.tar.gz` & `tmp/baal-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baal-1.7.0.tar", max compression
+gzip compressed data, was "baal-1.8.0.tar", max compression
```

## Comparing `baal-1.7.0.tar` & `baal-1.8.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    11357 2022-07-09 19:42:29.730723 baal-1.7.0/LICENSE
--rw-r--r--   0        0        0     7552 2022-10-28 21:52:52.692293 baal-1.7.0/README.md
--rw-r--r--   0        0        0      165 2022-07-09 19:42:29.730723 baal-1.7.0/baal/__init__.py
--rw-r--r--   0        0        0     1162 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/__init__.py
--rw-r--r--   0        0        0     3819 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/active_loop.py
--rw-r--r--   0        0        0      147 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/dataset/__init__.py
--rw-r--r--   0        0        0     4694 2022-08-20 15:06:46.551908 baal-1.7.0/baal/active/dataset/base.py
--rw-r--r--   0        0        0     3715 2022-08-20 15:06:46.551908 baal-1.7.0/baal/active/dataset/nlp_datasets.py
--rw-r--r--   0        0        0     2656 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/dataset/numpy.py
--rw-r--r--   0        0        0     9423 2022-10-28 21:52:52.696293 baal-1.7.0/baal/active/dataset/pytorch_dataset.py
--rw-r--r--   0        0        0     3043 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/file_dataset.py
--rw-r--r--   0        0        0       26 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/heuristics/__init__.py
--rw-r--r--   0        0        0    23579 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/heuristics/heuristics.py
--rw-r--r--   0        0        0     4532 2022-08-20 15:06:46.551908 baal-1.7.0/baal/active/heuristics/heuristics_gpu.py
--rw-r--r--   0        0        0     5698 2022-07-09 19:42:29.730723 baal-1.7.0/baal/active/heuristics/stochastics.py
--rw-r--r--   0        0        0      127 2022-07-09 19:42:29.730723 baal-1.7.0/baal/bayesian/__init__.py
--rw-r--r--   0        0        0     1809 2022-07-09 19:42:29.730723 baal-1.7.0/baal/bayesian/common.py
--rw-r--r--   0        0        0     5332 2022-07-09 19:42:29.730723 baal-1.7.0/baal/bayesian/consistent_dropout.py
--rw-r--r--   0        0        0     5418 2022-07-09 19:42:29.730723 baal-1.7.0/baal/bayesian/dropout.py
--rw-r--r--   0        0        0     5914 2022-07-09 19:42:29.734723 baal-1.7.0/baal/bayesian/weight_drop.py
--rw-r--r--   0        0        0       45 2022-07-09 19:42:29.734723 baal-1.7.0/baal/calibration/__init__.py
--rw-r--r--   0        0        0     5056 2022-08-20 15:06:46.551908 baal-1.7.0/baal/calibration/calibration.py
--rw-r--r--   0        0        0     2469 2022-07-09 19:42:29.734723 baal-1.7.0/baal/ensemble.py
--rw-r--r--   0        0        0        0 2022-08-21 16:32:48.317380 baal-1.7.0/baal/metrics/__init__.py
--rw-r--r--   0        0        0     3108 2022-10-28 21:52:52.696293 baal-1.7.0/baal/metrics/mixin.py
--rw-r--r--   0        0        0    16699 2022-10-28 21:52:52.696293 baal-1.7.0/baal/modelwrapper.py
--rw-r--r--   0        0        0     4995 2022-08-20 15:06:46.551908 baal-1.7.0/baal/transformers_trainer_wrapper.py
--rw-r--r--   0        0        0      760 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/__init__.py
--rw-r--r--   0        0        0     1569 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/array_utils.py
--rw-r--r--   0        0        0     2098 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/cuda_utils.py
--rw-r--r--   0        0        0      674 2022-10-28 21:52:52.696293 baal-1.7.0/baal/utils/equality.py
--rw-r--r--   0        0        0      296 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/iterutils.py
--rw-r--r--   0        0        0     3371 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/log_configuration.py
--rw-r--r--   0        0        0    16693 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/metrics.py
--rw-r--r--   0        0        0     3029 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/plot_utils.py
--rw-r--r--   0        0        0     7836 2022-08-21 16:32:48.321380 baal-1.7.0/baal/utils/pytorch_lightning.py
--rw-r--r--   0        0        0     5903 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/ssl_iterator.py
--rw-r--r--   0        0        0     2532 2022-08-20 15:06:46.551908 baal-1.7.0/baal/utils/ssl_module.py
--rw-r--r--   0        0        0     2579 2022-07-09 19:42:29.734723 baal-1.7.0/baal/utils/transforms.py
--rw-r--r--   0        0        0     1750 2022-10-28 21:53:15.268456 baal-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     8998 2022-10-28 21:53:48.702385 baal-1.7.0/setup.py
--rw-r--r--   0        0        0     8957 2022-10-28 21:53:48.703149 baal-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-09 19:42:29.730723 baal-1.8.0/LICENSE
+-rw-r--r--   0        0        0     7562 2023-07-13 22:01:39.835195 baal-1.8.0/README.md
+-rw-r--r--   0        0        0      165 2022-07-09 19:42:29.730723 baal-1.8.0/baal/__init__.py
+-rw-r--r--   0        0        0     1162 2022-07-09 19:42:29.730723 baal-1.8.0/baal/active/__init__.py
+-rw-r--r--   0        0        0     3819 2022-07-09 19:42:29.730723 baal-1.8.0/baal/active/active_loop.py
+-rw-r--r--   0        0        0      147 2022-07-09 19:42:29.730723 baal-1.8.0/baal/active/dataset/__init__.py
+-rw-r--r--   0        0        0     4931 2023-07-13 22:01:48.579265 baal-1.8.0/baal/active/dataset/base.py
+-rw-r--r--   0        0        0     3715 2022-08-20 15:06:46.551908 baal-1.8.0/baal/active/dataset/nlp_datasets.py
+-rw-r--r--   0        0        0     2713 2023-07-13 22:01:48.579265 baal-1.8.0/baal/active/dataset/numpy.py
+-rw-r--r--   0        0        0     9423 2022-10-28 21:52:52.696293 baal-1.8.0/baal/active/dataset/pytorch_dataset.py
+-rw-r--r--   0        0        0     3043 2022-07-09 19:42:29.730723 baal-1.8.0/baal/active/file_dataset.py
+-rw-r--r--   0        0        0       26 2022-07-09 19:42:29.730723 baal-1.8.0/baal/active/heuristics/__init__.py
+-rw-r--r--   0        0        0    24150 2023-07-13 20:31:16.340573 baal-1.8.0/baal/active/heuristics/heuristics.py
+-rw-r--r--   0        0        0     4532 2022-08-20 15:06:46.551908 baal-1.8.0/baal/active/heuristics/heuristics_gpu.py
+-rw-r--r--   0        0        0     5698 2022-07-09 19:42:29.730723 baal-1.8.0/baal/active/heuristics/stochastics.py
+-rw-r--r--   0        0        0      127 2022-07-09 19:42:29.730723 baal-1.8.0/baal/bayesian/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-13 22:01:48.579265 baal-1.8.0/baal/bayesian/caching_utils.py
+-rw-r--r--   0        0        0     1880 2023-03-04 15:23:50.812969 baal-1.8.0/baal/bayesian/common.py
+-rw-r--r--   0        0        0     5332 2022-07-09 19:42:29.730723 baal-1.8.0/baal/bayesian/consistent_dropout.py
+-rw-r--r--   0        0        0     5418 2022-07-09 19:42:29.730723 baal-1.8.0/baal/bayesian/dropout.py
+-rw-r--r--   0        0        0     5914 2022-07-09 19:42:29.734723 baal-1.8.0/baal/bayesian/weight_drop.py
+-rw-r--r--   0        0        0       45 2022-07-09 19:42:29.734723 baal-1.8.0/baal/calibration/__init__.py
+-rw-r--r--   0        0        0     5056 2022-08-20 15:06:46.551908 baal-1.8.0/baal/calibration/calibration.py
+-rw-r--r--   0        0        0     2469 2022-07-09 19:42:29.734723 baal-1.8.0/baal/ensemble.py
+-rw-r--r--   0        0        0        0 2022-08-21 16:32:48.317380 baal-1.8.0/baal/metrics/__init__.py
+-rw-r--r--   0        0        0     3108 2022-10-28 21:52:52.696293 baal-1.8.0/baal/metrics/mixin.py
+-rw-r--r--   0        0        0    16986 2023-07-13 22:01:39.835195 baal-1.8.0/baal/modelwrapper.py
+-rw-r--r--   0        0        0     4995 2023-07-13 22:01:39.835195 baal-1.8.0/baal/transformers_trainer_wrapper.py
+-rw-r--r--   0        0        0      760 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/__init__.py
+-rw-r--r--   0        0        0     1569 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/array_utils.py
+-rw-r--r--   0        0        0     2098 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/cuda_utils.py
+-rw-r--r--   0        0        0      674 2022-10-28 21:52:52.696293 baal-1.8.0/baal/utils/equality.py
+-rw-r--r--   0        0        0      296 2023-07-13 22:01:39.835195 baal-1.8.0/baal/utils/iterutils.py
+-rw-r--r--   0        0        0     3371 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/log_configuration.py
+-rw-r--r--   0        0        0    16693 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/metrics.py
+-rw-r--r--   0        0        0     3029 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/plot_utils.py
+-rw-r--r--   0        0        0     7839 2023-05-16 01:02:37.489674 baal-1.8.0/baal/utils/pytorch_lightning.py
+-rw-r--r--   0        0        0     5903 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/ssl_iterator.py
+-rw-r--r--   0        0        0     2532 2022-08-20 15:06:46.551908 baal-1.8.0/baal/utils/ssl_module.py
+-rw-r--r--   0        0        0     2579 2022-07-09 19:42:29.734723 baal-1.8.0/baal/utils/transforms.py
+-rw-r--r--   0        0        0     1753 2023-07-13 22:01:39.835195 baal-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8988 2023-07-13 22:04:43.984403 baal-1.8.0/setup.py
+-rw-r--r--   0        0        0     8946 2023-07-13 22:04:43.985117 baal-1.8.0/PKG-INFO
```

### Comparing `baal-1.7.0/LICENSE` & `baal-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/README.md` & `baal-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img height=15% width=25% src="https://github.com/ElementAI/baal/blob/master/docs/_static/images/logo-with-bg-solid.png?raw=true">
+  <img height=15% width=25% src="https://i.imgur.com/Zdzb2QZ.png" style="max-width: 100%;border-radius: 25%;">
   <h1 align="center">Bayesian Active Learning (Baal)
    <br>
   <a href="https://github.com/baal-org/baal/actions/workflows/pythonci.yml">
     <img alt="Python CI" src="https://github.com/baal-org/baal/actions/workflows/pythonci.yml/badge.svg"/>
   </a>
   <a href="https://baal.readthedocs.io/en/latest/?badge=latest">
     <img alt="Documentation Status" src="https://readthedocs.org/projects/baal/badge/?version=latest"/>
@@ -20,51 +20,50 @@
   <a href="https://pepy.tech/project/baal">
     <img alt="Downloads" src="https://pepy.tech/badge/baal"/>
   </a>
 
   </h1>
 </p>
 
-
-Baal is an active learning library initially developed at
-[ElementAI](https://www.elementai.com/) (acquired by ServiceNow in 2021).
-
-Our goal is to support both industrial applications and research in active learning.
+Baal is an active learning library that supports both industrial applications and research usecases.
 
 Read the documentation at https://baal.readthedocs.io.
 
 Our paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes tips and tricks to make active learning
 usable in production.
 
 For a quick introduction to Baal and Bayesian active learning, please see these links:
 
-* [Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)
-* [User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)
-* [Bayesian active learning presentation](https://drive.google.com/file/d/13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)
+- [Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)
+- [User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)
+- [Bayesian active learning presentation](https://drive.google.com/file/d/13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)
+
+*Baal was initially developed at [ElementAI](https://www.elementai.com/) (acquired by ServiceNow in 2021), but is now independant.*
+
 
 ## Installation and requirements
 
-Baal requires `Python>=3.7`.
+Baal requires `Python>=3.8`.
 
 To install Baal using pip: `pip install baal`
 
 We use [Poetry](https://python-poetry.org/) as our package manager.
 To install Baal from source: `poetry install`
 
 ## Papers using Baal
 
-* [Bayesian active learning for production, a systematic study and a reusable library
+- [Bayesian active learning for production, a systematic study and a reusable library
   ](https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020)
-* [Synbols: Probing Learning Algorithms with Synthetic Datasets
+- [Synbols: Probing Learning Algorithms with Synthetic Datasets
   ](https://nips.cc/virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020)
-* [Can Active Learning Preemptively Mitigate Fairness Issues?
+- [Can Active Learning Preemptively Mitigate Fairness Issues?
   ](https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)
-* [Active learning with MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/2112.06586) (
+- [Active learning with MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/2112.06586) (
   Blok et al. 2021)
-* [Stochastic Batch Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)
+- [Stochastic Batch Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)
 
 # What is active learning?
 
 Active learning is a special case of machine learning in which a learning algorithm is able to interactively query the
 user (or some other information source) to obtain the desired outputs at new data points
 (to understand the concept in more depth, refer to our [tutorial](https://baal.readthedocs.io/en/latest/)).
 
@@ -102,49 +101,51 @@
 We provide a lightweight object _[**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it easier to
 train and test the model. If your model is not ready for active learning, we provide Modules to prepare them.
 
 For example, the _[**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing dropout layer to be used
 in both training and inference time and the `ModelWrapper` makes the specifies the number of iterations to run at
 training and inference.
 
+Finally, _[**ActiveLearningLoop**](baal/active/active_loop.py)_ automatically computes the uncertainty and label the most
+uncertain items in the pool.
+
 In conclusion, your script should be similar to this:
 
 ```python
 dataset = ActiveLearningDataset(your_dataset)
 dataset.label_randomly(INITIAL_POOL)  # label some data
 model = MCDropoutModule(your_model)
 model = ModelWrapper(model, your_criterion)
 active_loop = ActiveLearningLoop(dataset,
                                  get_probabilities=model.predict_on_dataset,
-                                 heuristic=heuristics.BALD(shuffle_prop=0.1),
-                                 query_size=NDATA_TO_LABEL)
+                                 heuristic=heuristics.BALD(),
+                                 iterations=20, # Number of MC sampling.
+                                 query_size=QUERY_SIZE)  # Number of item to label.
 for al_step in range(N_ALSTEP):
     model.train_on_dataset(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda)
+    metrics = model.test_on_dataset(test_dataset, BATCH_SIZE)
+    # Label the next most uncertain items.
     if not active_loop.step():
         # We're done!
         break
 ```
 
-For a complete experiment, we provide _[experiments/](experiments/)_ to understand how to write an active training
-process. Generally, we use the **ActiveLearningLoop**
-provided at _[src/baal/active/active_loop.py](baal/active/active_loop.py)_. This class provides functionality to get the
-predictions on the unlabeled pool after each (few) epoch(s) and sort the next set of data items to be labeled based on
-the calculated uncertainty of the pool.
+For a complete experiment, see _[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_ .
 
 ### Re-run our Experiments
 
 ```bash
 docker build [--target base_baal] -t baal .
-docker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py 
+docker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py
 ```
 
 ### Use Baal for YOUR Experiments
 
 Simply clone the repo, and create your own experiment script similar to the example
-at [experiments/vgg_experiment.py](experiments/vgg_experiment.py). Make sure to use the four main parts of Baal
+at _[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_. Make sure to use the four main parts of Baal
 framework. _Happy running experiments_
 
 ### Contributing!
 
 To contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md).
 
 ### Who We Are!
```

#### html2text {}

```diff
@@ -1,88 +1,85 @@
- [https://github.com/ElementAI/baal/blob/master/docs/_static/images/logo-with-
-                            bg-solid.png?raw=true]
+                       [https://i.imgur.com/Zdzb2QZ.png]
                     ****** Bayesian Active Learning (Baal)
 [Python_CI] [Documentation_Status] [Slack] [Licence] [Office_hours] [Downloads]
                                     ******
-Baal is an active learning library initially developed at [ElementAI](https://
-www.elementai.com/) (acquired by ServiceNow in 2021). Our goal is to support
-both industrial applications and research in active learning. Read the
-documentation at https://baal.readthedocs.io. Our paper can be read on [arXiv]
-(https://arxiv.org/abs/2006.09916). It includes tips and tricks to make active
-learning usable in production. For a quick introduction to Baal and Bayesian
-active learning, please see these links: * [Seminar with Label Studio](https://
-www.youtube.com/watch?v=HG7imRQN3-k) * [User guide](https://
-baal.readthedocs.io/en/latest/user_guide/index.html) * [Bayesian active
-learning presentation](https://drive.google.com/file/d/
-13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing) ## Installation and
-requirements Baal requires `Python>=3.7`. To install Baal using pip: `pip
-install baal` We use [Poetry](https://python-poetry.org/) as our package
-manager. To install Baal from source: `poetry install` ## Papers using Baal *
-[Bayesian active learning for production, a systematic study and a reusable
-library ](https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020) *
-[Synbols: Probing Learning Algorithms with Synthetic Datasets ](https://
-nips.cc/virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html)
-(Lacoste et al. 2020) * [Can Active Learning Preemptively Mitigate Fairness
-Issues? ](https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)
-* [Active learning with MaskAL reduces annotation effort for training Mask R-
-CNN](https://arxiv.org/abs/2112.06586) ( Blok et al. 2021) * [Stochastic Batch
-Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch
-et al. 2022) # What is active learning? Active learning is a special case of
-machine learning in which a learning algorithm is able to interactively query
-the user (or some other information source) to obtain the desired outputs at
-new data points (to understand the concept in more depth, refer to our
-[tutorial](https://baal.readthedocs.io/en/latest/)). ## Baal Framework At the
-moment Baal supports the following methods to perform active learning. - Monte-
-Carlo Dropout (Gal et al. 2015) - MCDropConnect (Mobiny et al. 2019) - Deep
-ensembles - Semi-supervised learning If you want to propose new methods, please
-submit an issue. The **Monte-Carlo Dropout** method is a known approximation
-for Bayesian neural networks. In this method, the Dropout layer is used both in
-training and test time. By running the model multiple times whilst randomly
-dropping weights, we calculate the uncertainty of the prediction using one of
-the uncertainty measurements in [heuristics.py](baal/active/heuristics/
-heuristics.py). The framework consists of four main parts, as demonstrated in
-the flowchart below: - ActiveLearningDataset - Heuristics - ModelWrapper -
-ActiveLearningLoop
+Baal is an active learning library that supports both industrial applications
+and research usecases. Read the documentation at https://baal.readthedocs.io.
+Our paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes
+tips and tricks to make active learning usable in production. For a quick
+introduction to Baal and Bayesian active learning, please see these links: -
+[Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k) -
+[User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html) -
+[Bayesian active learning presentation](https://drive.google.com/file/d/
+13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing) *Baal was initially
+developed at [ElementAI](https://www.elementai.com/) (acquired by ServiceNow in
+2021), but is now independant.* ## Installation and requirements Baal requires
+`Python>=3.8`. To install Baal using pip: `pip install baal` We use [Poetry]
+(https://python-poetry.org/) as our package manager. To install Baal from
+source: `poetry install` ## Papers using Baal - [Bayesian active learning for
+production, a systematic study and a reusable library ](https://arxiv.org/abs/
+2006.09916) (Atighehchian et al. 2020) - [Synbols: Probing Learning Algorithms
+with Synthetic Datasets ](https://nips.cc/virtual/2020/public/
+poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020) - [Can
+Active Learning Preemptively Mitigate Fairness Issues? ](https://arxiv.org/pdf/
+2104.06879.pdf) (Branchaud-Charron et al. 2021) - [Active learning with MaskAL
+reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/
+2112.06586) ( Blok et al. 2021) - [Stochastic Batch Acquisition for Deep Active
+Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022) # What is
+active learning? Active learning is a special case of machine learning in which
+a learning algorithm is able to interactively query the user (or some other
+information source) to obtain the desired outputs at new data points (to
+understand the concept in more depth, refer to our [tutorial](https://
+baal.readthedocs.io/en/latest/)). ## Baal Framework At the moment Baal supports
+the following methods to perform active learning. - Monte-Carlo Dropout (Gal et
+al. 2015) - MCDropConnect (Mobiny et al. 2019) - Deep ensembles - Semi-
+supervised learning If you want to propose new methods, please submit an issue.
+The **Monte-Carlo Dropout** method is a known approximation for Bayesian neural
+networks. In this method, the Dropout layer is used both in training and test
+time. By running the model multiple times whilst randomly dropping weights, we
+calculate the uncertainty of the prediction using one of the uncertainty
+measurements in [heuristics.py](baal/active/heuristics/heuristics.py). The
+framework consists of four main parts, as demonstrated in the flowchart below:
+- ActiveLearningDataset - Heuristics - ModelWrapper - ActiveLearningLoop
                [docs/research/literature/images/Baalscheme.svg]
 To get started, wrap your dataset in our _[**ActiveLearningDataset**](baal/
 active/dataset.py)_ class. This will ensure that the dataset is split into
 `training` and `pool` sets. The `pool` set represents the portion of the
 training set which is yet to be labelled. We provide a lightweight object _
 [**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it
 easier to train and test the model. If your model is not ready for active
 learning, we provide Modules to prepare them. For example, the _
 [**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing
 dropout layer to be used in both training and inference time and the
 `ModelWrapper` makes the specifies the number of iterations to run at training
-and inference. In conclusion, your script should be similar to this: ```python
+and inference. Finally, _[**ActiveLearningLoop**](baal/active/active_loop.py)_
+automatically computes the uncertainty and label the most uncertain items in
+the pool. In conclusion, your script should be similar to this: ```python
 dataset = ActiveLearningDataset(your_dataset) dataset.label_randomly
 (INITIAL_POOL) # label some data model = MCDropoutModule(your_model) model =
 ModelWrapper(model, your_criterion) active_loop = ActiveLearningLoop(dataset,
-get_probabilities=model.predict_on_dataset, heuristic=heuristics.BALD
-(shuffle_prop=0.1), query_size=NDATA_TO_LABEL) for al_step in range(N_ALSTEP):
-model.train_on_dataset(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda) if
-not active_loop.step(): # We're done! break ``` For a complete experiment, we
-provide _[experiments/](experiments/)_ to understand how to write an active
-training process. Generally, we use the **ActiveLearningLoop** provided at _
-[src/baal/active/active_loop.py](baal/active/active_loop.py)_. This class
-provides functionality to get the predictions on the unlabeled pool after each
-(few) epoch(s) and sort the next set of data items to be labeled based on the
-calculated uncertainty of the pool. ### Re-run our Experiments ```bash docker
-build [--target base_baal] -t baal . docker run --rm baal --gpus all python3
-experiments/vgg_mcdropout_cifar10.py ``` ### Use Baal for YOUR Experiments
-Simply clone the repo, and create your own experiment script similar to the
-example at [experiments/vgg_experiment.py](experiments/vgg_experiment.py). Make
-sure to use the four main parts of Baal framework. _Happy running experiments_
-### Contributing! To contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md). ###
-Who We Are! "There is passion, yet peace; serenity, yet emotion; chaos, yet
-order." The Baal team tests and implements the most recent papers on
-uncertainty estimation and active learning. Current maintainers: - [Parmida
-Atighehchian](mailto:patighehchian@twitter.com) - [FrÃ©dÃ©ric Branchaud-
-Charron](mailto:frederic.branchaud-charron@gmail.com) - [George Pearse]
-(georgehwp26@gmail.com) ### How to cite If you used Baal in one of your
-project, we would greatly appreciate if you cite this library using this
-Bibtex: ``` @misc{atighehchian2019baal, title={Baal, a bayesian active learning
-library}, author={Atighehchian, Parmida and Branchaud-Charron, Frederic and
-Freyberg, Jan and Pardinas, Rafael and Schell, Lorne and Pearse, George}, year=
-{2022}, howpublished={\url{https://github.com/baal-org/baal/}}, } ``` ###
-Licence To get information on licence of this API please read [LICENCE](./
-LICENSE)
+get_probabilities=model.predict_on_dataset, heuristic=heuristics.BALD(),
+iterations=20, # Number of MC sampling. query_size=QUERY_SIZE) # Number of item
+to label. for al_step in range(N_ALSTEP): model.train_on_dataset(dataset,
+optimizer, BATCH_SIZE, use_cuda=use_cuda) metrics = model.test_on_dataset
+(test_dataset, BATCH_SIZE) # Label the next most uncertain items. if not
+active_loop.step(): # We're done! break ``` For a complete experiment, see _
+[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_ .
+### Re-run our Experiments ```bash docker build [--target base_baal] -t baal .
+docker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py
+``` ### Use Baal for YOUR Experiments Simply clone the repo, and create your
+own experiment script similar to the example at _[experiments/
+vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_. Make sure to
+use the four main parts of Baal framework. _Happy running experiments_ ###
+Contributing! To contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md). ### Who
+We Are! "There is passion, yet peace; serenity, yet emotion; chaos, yet order."
+The Baal team tests and implements the most recent papers on uncertainty
+estimation and active learning. Current maintainers: - [Parmida Atighehchian]
+(mailto:patighehchian@twitter.com) - [FrÃ©dÃ©ric Branchaud-Charron](mailto:
+frederic.branchaud-charron@gmail.com) - [George Pearse](georgehwp26@gmail.com)
+### How to cite If you used Baal in one of your project, we would greatly
+appreciate if you cite this library using this Bibtex: ``` @misc
+{atighehchian2019baal, title={Baal, a bayesian active learning library},
+author={Atighehchian, Parmida and Branchaud-Charron, Frederic and Freyberg, Jan
+and Pardinas, Rafael and Schell, Lorne and Pearse, George}, year={2022},
+howpublished={\url{https://github.com/baal-org/baal/}}, } ``` ### Licence To
+get information on licence of this API please read [LICENCE](./LICENSE)
```

### Comparing `baal-1.7.0/baal/active/__init__.py` & `baal-1.8.0/baal/active/__init__.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/active/active_loop.py` & `baal-1.8.0/baal/active/active_loop.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/active/dataset/base.py` & `baal-1.8.0/baal/active/dataset/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,31 +36,36 @@
         last_active_steps: int = -1,
     ) -> None:
         self.labelled_map = labelled
         self.random_state = check_random_state(random_state)
         if last_active_steps == 0 or last_active_steps < -1:
             raise ValueError("last_active_steps must be > 0 or -1 when disabled.")
         self.last_active_steps = last_active_steps
+        self._indices_cache = (-1, None)
 
     def get_indices_for_active_step(self) -> List[int]:
         """Returns the indices required for the active step.
 
         Returns the indices of the labelled items. Also takes into account self.last_active_step.
 
         Returns:
             List of the selected indices for training.
         """
-        if self.last_active_steps == -1:
-            min_labelled_step = 0
-        else:
-            min_labelled_step = max(0, self.current_al_step - self.last_active_steps)
-
-        # we need to work with lists since arrow dataset is not compatible with np.int types!
-        indices = [indx for indx, val in enumerate(self.labelled_map) if val > min_labelled_step]
-        return indices
+        if (curr_al_step := self.current_al_step) != self._indices_cache[0]:
+            if self.last_active_steps == -1:
+                min_labelled_step = 0
+            else:
+                min_labelled_step = max(0, curr_al_step - self.last_active_steps)
+
+            # we need to work with lists since arrow dataset is not compatible with np.int types!
+            indices = [
+                indx for indx, val in enumerate(self.labelled_map) if val > min_labelled_step
+            ]
+            self._indices_cache = (curr_al_step, indices)
+        return self._indices_cache[1]
 
     def is_labelled(self, idx: int) -> bool:
         """Check if a datapoint is labelled."""
         return bool(self.labelled[idx].item() == 1)
 
     def __len__(self) -> int:
         """Return how many actual data / label pairs we have."""
```

### Comparing `baal-1.7.0/baal/active/dataset/nlp_datasets.py` & `baal-1.8.0/baal/active/dataset/nlp_datasets.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/active/dataset/numpy.py` & `baal-1.8.0/baal/active/dataset/numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,9 +64,10 @@
                                     to the underlying dataset is done.
         """
         if isinstance(index, int):
             index = [index]
         if not isinstance(value, (list, tuple)):
             value = [value]
         indexes = self._pool_to_oracle_index(index)
+        active_step = self.current_al_step + 1
         for index, val in zip_longest(indexes, value, fillvalue=None):
-            self.labelled_map[index] = 1
+            self.labelled_map[index] = active_step
```

### Comparing `baal-1.7.0/baal/active/dataset/pytorch_dataset.py` & `baal-1.8.0/baal/active/dataset/pytorch_dataset.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/active/file_dataset.py` & `baal-1.8.0/baal/active/file_dataset.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/active/heuristics/heuristics.py` & `baal-1.8.0/baal/active/heuristics/heuristics.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 import scipy.stats
 import torch
 from scipy.special import xlogy
 from torch import Tensor
 
 from baal.utils.array_utils import to_prob
 
+DEPRECATED = "DEPRECATED"
+SHUFFLE_PROP_DEPRECATION_NOTICE = """
+`shuffle_prop` is deprecated and will be removed in Baal 1.9.0.
+For better batch uncertainty estimation, use `baal.active.heuristics.stochastics.PowerSampling`.
+See `https://baal.readthedocs.io/en/latest/user_guide/heuristics/` for more details.
+"""
+
 available_reductions = {
     "max": lambda x: np.max(x, axis=tuple(range(1, x.ndim))),
     "min": lambda x: np.min(x, axis=tuple(range(1, x.ndim))),
     "mean": lambda x: np.mean(x, axis=tuple(range(1, x.ndim))),
     "sum": lambda x: np.sum(x, axis=tuple(range(1, x.ndim))),
     "none": lambda x: x,
 }
@@ -135,15 +142,19 @@
 
     Args:
         shuffle_prop (float): shuffle proportion.
         reverse (bool): True if the most uncertain sample has the highest value.
         reduction (Union[str, Callable]): Reduction used after computing the score.
     """
 
-    def __init__(self, shuffle_prop=0.0, reverse=False, reduction="none"):
+    def __init__(self, shuffle_prop=DEPRECATED, reverse=False, reduction="none"):
+        if shuffle_prop != DEPRECATED and shuffle_prop < 1.0:
+            warnings.warn(SHUFFLE_PROP_DEPRECATION_NOTICE, DeprecationWarning)
+        else:
+            shuffle_prop = 0.0
         self.shuffle_prop = shuffle_prop
         self.reversed = reverse
         assert reduction in available_reductions or callable(reduction)
         self._reduction_name = reduction
         self.reduction = reduction if callable(reduction) else available_reductions[reduction]
 
     def compute_score(self, predictions):
@@ -268,15 +279,15 @@
         reduction (Union[str, callable]): function that aggregates the results
             (default: 'none`).
 
     References:
         https://arxiv.org/abs/1703.02910
     """
 
-    def __init__(self, shuffle_prop=0.0, reduction="none"):
+    def __init__(self, shuffle_prop=DEPRECATED, reduction="none"):
         super().__init__(shuffle_prop=shuffle_prop, reverse=True, reduction=reduction)
 
     @require_single_item
     @requireprobs
     def compute_score(self, predictions):
         """
         Compute the score according to the heuristic.
@@ -320,15 +331,15 @@
         https://arxiv.org/abs/1906.08158
 
     Notes:
         K = iterations, C=classes
         Not tested on 4+ dims.
     """
 
-    def __init__(self, num_samples, num_draw=500, shuffle_prop=0.0, reduction="none"):
+    def __init__(self, num_samples, num_draw=500, shuffle_prop=DEPRECATED, reduction="none"):
         self.epsilon = 1e-5
         self.num_samples = num_samples
         self.num_draw = num_draw
         super().__init__(shuffle_prop=shuffle_prop, reduction=reduction)
 
     def _draw_choices(self, probs, n_choices):
         """
@@ -504,15 +515,15 @@
 
     Args:
         shuffle_prop (float): Amount of noise to put in the ranking. Helps with selection bias
             (default: 0.0).
         reduction (Union[str, callable]): function that aggregates the results (default: `mean`).
     """
 
-    def __init__(self, shuffle_prop=0.0, reduction="mean"):
+    def __init__(self, shuffle_prop=DEPRECATED, reduction="mean"):
         _help = "Need to reduce the output from [n_sample, n_class] to [n_sample]"
         assert reduction != "none", _help
         super().__init__(shuffle_prop=shuffle_prop, reverse=True, reduction=reduction)
 
     @require_single_item
     def compute_score(self, predictions):
         assert predictions.ndim >= 3
@@ -525,15 +536,15 @@
 
     Args:
         shuffle_prop (float): Amount of noise to put in the ranking. Helps with selection bias
             (default: 0.0).
         reduction (Union[str, callable]): function that aggregates the results (default: `none`).
     """
 
-    def __init__(self, shuffle_prop=0.0, reduction="none"):
+    def __init__(self, shuffle_prop=DEPRECATED, reduction="none"):
         super().__init__(shuffle_prop=shuffle_prop, reverse=True, reduction=reduction)
 
     @require_single_item
     @singlepass
     @requireprobs
     def compute_score(self, predictions):
         return scipy.stats.entropy(np.swapaxes(predictions, 0, 1))
@@ -547,15 +558,15 @@
     Args:
         shuffle_prop (float): Amount of noise to put in the ranking. Helps with selection bias
             (default: 0.0).
         reduction (Union[str, callable]): function that aggregates the results
             (default: `none`).
     """
 
-    def __init__(self, shuffle_prop=0.0, reduction="none"):
+    def __init__(self, shuffle_prop=DEPRECATED, reduction="none"):
         super().__init__(shuffle_prop=shuffle_prop, reverse=False, reduction=reduction)
 
     @require_single_item
     @singlepass
     @requireprobs
     def compute_score(self, predictions):
         sort_arr = np.sort(predictions, axis=1)
@@ -567,15 +578,15 @@
     Sort by the lowest certainty.
 
     Args:
         shuffle_prop (float): Amount of noise to put in the ranking. Helps with selection bias.
         reduction (Union[str, callable]): function that aggregates the results.
     """
 
-    def __init__(self, shuffle_prop=0.0, reduction="none"):
+    def __init__(self, shuffle_prop=DEPRECATED, reduction="none"):
         super().__init__(shuffle_prop=shuffle_prop, reverse=False, reduction=reduction)
 
     @require_single_item
     @singlepass
     def compute_score(self, predictions):
         return np.max(predictions, axis=1)
 
@@ -584,15 +595,15 @@
     """Precomputed heuristics.
 
     Args:
         shuffle_prop (float): Amount of noise to put in the ranking. Helps with selection bias.
         reverse (Bool): Sort from lowest to highest if False.
     """
 
-    def __init__(self, shuffle_prop=0.0, reverse=False):
+    def __init__(self, shuffle_prop=DEPRECATED, reverse=False):
         super().__init__(shuffle_prop, reverse=reverse)
 
     def compute_score(self, predictions):
         return predictions
 
 
 class Random(Precomputed):
@@ -600,15 +611,15 @@
 
     Args:
         shuffle_prop (float): UNUSED
         reduction (Union[str, callable]): UNUSED.
         seed (Optional[int]): If provided, will seed the random generator.
     """
 
-    def __init__(self, shuffle_prop=0.0, reduction="none", seed=None):
+    def __init__(self, shuffle_prop=DEPRECATED, reduction="none", seed=None):
         super().__init__(1.0, False)
         if seed is not None:
             self.rng = np.random.RandomState(seed)
         else:
             self.rng = np.random
 
     def compute_score(self, predictions):
@@ -639,15 +650,15 @@
             before calculation of ranks
         reduction (Union[str, callable]): function that aggregates the results of the heuristics
             (default: weighted average which could be used as (reduction='mean`)
        shuffle_prop (float): shuffle proportion.
 
     """
 
-    def __init__(self, heuristics: List, weights: List, reduction="mean", shuffle_prop=0.0):
+    def __init__(self, heuristics: List, weights: List, reduction="mean", shuffle_prop=DEPRECATED):
         super(CombineHeuristics, self).__init__(reduction=reduction, shuffle_prop=shuffle_prop)
         self.composed_heuristic = heuristics
         self.weights = weights
         reversed = [bool(heuristic.reversed) for heuristic in self.composed_heuristic]
 
         if all(item is False for item in reversed):
             self.reversed = False
```

### Comparing `baal-1.7.0/baal/active/heuristics/heuristics_gpu.py` & `baal-1.8.0/baal/active/heuristics/heuristics_gpu.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/active/heuristics/stochastics.py` & `baal-1.8.0/baal/active/heuristics/stochastics.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/bayesian/common.py` & `baal-1.8.0/baal/bayesian/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     Recursively iterate over the children of a module and replace them according to `mapping_fn`.
 
     Returns:
         True if a layer has been changed.
     """
     changed = False
     for name, child in module.named_children():
-        new_module = mapping_fn(child, *args, **kwargs)
+        new_module: Optional[nn.Module] = mapping_fn(child, *args, **kwargs)
 
         if new_module is not None:
             changed = True
+            new_module.train(mode=child.training)
             module.add_module(name, new_module)
 
         # recursively apply to child
         changed |= replace_layers_in_module(child, mapping_fn, *args, **kwargs)
     return changed
```

### Comparing `baal-1.7.0/baal/bayesian/consistent_dropout.py` & `baal-1.8.0/baal/bayesian/consistent_dropout.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/bayesian/dropout.py` & `baal-1.8.0/baal/bayesian/dropout.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/bayesian/weight_drop.py` & `baal-1.8.0/baal/bayesian/weight_drop.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/calibration/calibration.py` & `baal-1.8.0/baal/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/ensemble.py` & `baal-1.8.0/baal/ensemble.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/metrics/mixin.py` & `baal-1.8.0/baal/metrics/mixin.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/modelwrapper.py` & `baal-1.8.0/baal/modelwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         use_cuda: bool,
         workers: int = 4,
         collate_fn: Optional[Callable] = None,
         regularizer: Optional[Callable] = None,
         return_best_weights=False,
         patience=None,
         min_epoch_for_es=0,
+        skip_epochs=1,
     ):
         """
         Train and test the model on both Dataset `train_dataset`, `test_dataset`.
 
         Args:
             train_dataset (Dataset): Dataset to train on.
             test_dataset (Dataset): Dataset to evaluate on.
@@ -162,37 +163,43 @@
             workers (int): Number of workers to use.
             collate_fn (Optional[Callable]): The collate function to use.
             regularizer (Optional[Callable]): The loss regularization for training.
             return_best_weights (bool): If True, will keep the best weights and return them.
             patience (Optional[int]): If provided, will use early stopping to stop after
                                         `patience` epoch without improvement.
             min_epoch_for_es (int): Epoch at which the early stopping starts.
+            skip_epochs (int): Number of epochs to skip for test_on_dataset
 
         Returns:
             History and best weights if required.
         """
         best_weight = None
         best_loss = 1e10
         best_epoch = 0
         hist = []
         for e in range(epoch):
             _ = self.train_on_dataset(
                 train_dataset, optimizer, batch_size, 1, use_cuda, workers, collate_fn, regularizer
             )
-            te_loss = self.test_on_dataset(test_dataset, batch_size, use_cuda, workers, collate_fn)
-            hist.append(self.get_metrics())
-            if te_loss < best_loss:
-                best_epoch = e
-                best_loss = te_loss
-                if return_best_weights:
-                    best_weight = deepcopy(self.state_dict())
+            if e % skip_epochs == 0:
+                te_loss = self.test_on_dataset(
+                    test_dataset, batch_size, use_cuda, workers, collate_fn
+                )
+                hist.append(self.get_metrics())
+                if te_loss < best_loss:
+                    best_epoch = e
+                    best_loss = te_loss
+                    if return_best_weights:
+                        best_weight = deepcopy(self.state_dict())
 
-            if patience is not None and (e - best_epoch) > patience and (e > min_epoch_for_es):
-                # Early stopping
-                break
+                if patience is not None and (e - best_epoch) > patience and (e > min_epoch_for_es):
+                    # Early stopping
+                    break
+            else:
+                hist.append(self.get_metrics("train"))
 
         if return_best_weights:
             return hist, best_weight
         else:
             return hist
 
     def predict_on_dataset_generator(
```

### Comparing `baal-1.7.0/baal/transformers_trainer_wrapper.py` & `baal-1.8.0/baal/transformers_trainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/__init__.py` & `baal-1.8.0/baal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/array_utils.py` & `baal-1.8.0/baal/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/cuda_utils.py` & `baal-1.8.0/baal/utils/cuda_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/equality.py` & `baal-1.8.0/baal/utils/equality.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/log_configuration.py` & `baal-1.8.0/baal/utils/log_configuration.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/metrics.py` & `baal-1.8.0/baal/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/plot_utils.py` & `baal-1.8.0/baal/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/pytorch_lightning.py` & `baal-1.8.0/baal/utils/pytorch_lightning.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Sequence
 from typing import Dict, Any, Optional
 
 import numpy as np
 import structlog
 import torch
 from pytorch_lightning import Trainer, Callback, LightningDataModule, LightningModule
-from pytorch_lightning.accelerators import GPUAccelerator
+from pytorch_lightning.accelerators import CUDAAccelerator
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from baal.active import ActiveLearningDataset
 from baal.active.heuristics import heuristics
 from baal.modelwrapper import mc_inference
 from baal.utils.cuda_utils import to_cuda
@@ -148,23 +148,23 @@
                                                 Otherwise, uses model.pool_dataloader().
 
         Returns:
             Numpy arrays with all the predictions.
         """
         model = model or self.lightning_module
         model.eval()
-        if isinstance(self.accelerator, GPUAccelerator):
+        if isinstance(self.accelerator, CUDAAccelerator):
             model.cuda(self.strategy.root_device.index)
         dataloader = dataloader or model.pool_dataloader()
         if len(dataloader) == 0:
             return None
 
         log.info("Start Predict", dataset=len(dataloader))
         for idx, batch in enumerate(tqdm(dataloader, total=len(dataloader), file=sys.stdout)):
-            if isinstance(self.accelerator, GPUAccelerator):
+            if isinstance(self.accelerator, CUDAAccelerator):
                 batch = to_cuda(batch)
             pred = model.predict_step(batch, idx)
             yield map_on_tensor(lambda x: x.detach().cpu().numpy(), pred)
         # teardown, TODO customize this later?
         model.cpu()
 
     def step(self, model=None, datamodule: Optional[BaaLDataModule] = None) -> bool:
```

### Comparing `baal-1.7.0/baal/utils/ssl_iterator.py` & `baal-1.8.0/baal/utils/ssl_iterator.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/ssl_module.py` & `baal-1.8.0/baal/utils/ssl_module.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/baal/utils/transforms.py` & `baal-1.8.0/baal/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `baal-1.7.0/pyproject.toml` & `baal-1.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baal"
-version = "1.7.0"
+version = "1.8.0"
 description = "Library to enable Bayesian active learning in your research or labeling work."
 authors = ["Parmida Atighehchian <parmida.atighehchian@servicenow.com>",
            "Frederic Branchaud-Charron <frederic.branchaud-charron@servicenow.com>",
            "Jan Freyberg <jan.freyberg@gmail.com>",
            "Lorne Schell <lorne.schell@servicenow.com>",
            "Rafael Pardina <rafael.pardinas@servicenow.com>"
            ]
@@ -24,28 +24,28 @@
 tqdm = "^4.62.2"
 structlog = "^21.1.0"
 scikit-learn = "^1.0.0"
 scipy = "^1.7.1"
 
 # Vision
 torchvision = { version = ">=0.7.0", optional=true }
-lightning-flash = { version = "^0.7.5", optional=true }
+lightning-flash = { version = ">=0.7.5", optional=true }
 
 # NLP
-transformers = {version = "^4.10.2", optional=true}
-datasets = {version = "^1.11.0", optional=true}
+transformers = {version = ">=4.10.2", optional=true}
+datasets = {version = ">=1.11.0", optional=true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
 torch-hypothesis = "0.2.0"
 hypothesis = "4.24.0"
 flake8 = "^3.9.2"
 pytest-mock = "^3.6.1"
-black = "^21.8b0"
+black = "^22.3.0"
 mypy = "^0.910"
 bandit = "^1.7.1"
 
 # Documentation
 docutils = "0.16"
 
 # Documentation
```

### Comparing `baal-1.7.0/setup.py` & `baal-1.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,22 +23,22 @@
  'scipy>=1.7.1,<2.0.0',
  'structlog>=21.1.0,<22.0.0',
  'torch>=1.6.0',
  'torchmetrics>=0.9.3,<0.10.0',
  'tqdm>=4.62.2,<5.0.0']
 
 extras_require = \
-{'nlp': ['transformers>=4.10.2,<5.0.0', 'datasets>=1.11.0,<2.0.0'],
- 'vision': ['torchvision>=0.7.0', 'lightning-flash>=0.7.5,<0.8.0']}
+{'nlp': ['transformers>=4.10.2', 'datasets>=1.11.0'],
+ 'vision': ['torchvision>=0.7.0', 'lightning-flash>=0.7.5']}
 
 setup_kwargs = {
     'name': 'baal',
-    'version': '1.7.0',
+    'version': '1.8.0',
     'description': 'Library to enable Bayesian active learning in your research or labeling work.',
-    'long_description': '<p align="center">\n  <img height=15% width=25% src="https://github.com/ElementAI/baal/blob/master/docs/_static/images/logo-with-bg-solid.png?raw=true">\n  <h1 align="center">Bayesian Active Learning (Baal)\n   <br>\n  <a href="https://github.com/baal-org/baal/actions/workflows/pythonci.yml">\n    <img alt="Python CI" src="https://github.com/baal-org/baal/actions/workflows/pythonci.yml/badge.svg"/>\n  </a>\n  <a href="https://baal.readthedocs.io/en/latest/?badge=latest">\n    <img alt="Documentation Status" src="https://readthedocs.org/projects/baal/badge/?version=latest"/>\n  </a>\n  <a href="https://join.slack.com/t/baal-world/shared_invite/zt-z0izhn4y-Jt6Zu5dZaV2rsAS9sdISfg">\n    <img alt="Slack" src="https://img.shields.io/badge/slack-chat-green.svg?logo=slack"/>\n  </a>\n  <a href="https://github.com/Elementai/baal/blob/master/LICENSE">\n    <img alt="Licence" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/>\n  </a>\n  <a href="https://calendly.com/baal-org/30min">\n    <img alt="Office hours" src="https://img.shields.io/badge/Office hours-Calendly-blue.svg"/>\n  </a>\n  <a href="https://pepy.tech/project/baal">\n    <img alt="Downloads" src="https://pepy.tech/badge/baal"/>\n  </a>\n\n  </h1>\n</p>\n\n\nBaal is an active learning library initially developed at\n[ElementAI](https://www.elementai.com/) (acquired by ServiceNow in 2021).\n\nOur goal is to support both industrial applications and research in active learning.\n\nRead the documentation at https://baal.readthedocs.io.\n\nOur paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes tips and tricks to make active learning\nusable in production.\n\nFor a quick introduction to Baal and Bayesian active learning, please see these links:\n\n* [Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)\n* [User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)\n* [Bayesian active learning presentation](https://drive.google.com/file/d/13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)\n\n## Installation and requirements\n\nBaal requires `Python>=3.7`.\n\nTo install Baal using pip: `pip install baal`\n\nWe use [Poetry](https://python-poetry.org/) as our package manager.\nTo install Baal from source: `poetry install`\n\n## Papers using Baal\n\n* [Bayesian active learning for production, a systematic study and a reusable library\n  ](https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020)\n* [Synbols: Probing Learning Algorithms with Synthetic Datasets\n  ](https://nips.cc/virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020)\n* [Can Active Learning Preemptively Mitigate Fairness Issues?\n  ](https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)\n* [Active learning with MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/2112.06586) (\n  Blok et al. 2021)\n* [Stochastic Batch Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)\n\n# What is active learning?\n\nActive learning is a special case of machine learning in which a learning algorithm is able to interactively query the\nuser (or some other information source) to obtain the desired outputs at new data points\n(to understand the concept in more depth, refer to our [tutorial](https://baal.readthedocs.io/en/latest/)).\n\n## Baal Framework\n\nAt the moment Baal supports the following methods to perform active learning.\n\n- Monte-Carlo Dropout (Gal et al. 2015)\n- MCDropConnect (Mobiny et al. 2019)\n- Deep ensembles\n- Semi-supervised learning\n\nIf you want to propose new methods, please submit an issue.\n\nThe **Monte-Carlo Dropout** method is a known approximation for Bayesian neural networks. In this method, the Dropout\nlayer is used both in training and test time. By running the model multiple times whilst randomly dropping weights, we\ncalculate the uncertainty of the prediction using one of the uncertainty measurements\nin [heuristics.py](baal/active/heuristics/heuristics.py).\n\nThe framework consists of four main parts, as demonstrated in the flowchart below:\n\n- ActiveLearningDataset\n- Heuristics\n- ModelWrapper\n- ActiveLearningLoop\n\n<p align="center">\n  <img src="docs/research/literature/images/Baalscheme.svg">\n</p>\n\nTo get started, wrap your dataset in our _[**ActiveLearningDataset**](baal/active/dataset.py)_ class. This will ensure\nthat the dataset is split into\n`training` and `pool` sets. The `pool` set represents the portion of the training set which is yet to be labelled.\n\nWe provide a lightweight object _[**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it easier to\ntrain and test the model. If your model is not ready for active learning, we provide Modules to prepare them.\n\nFor example, the _[**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing dropout layer to be used\nin both training and inference time and the `ModelWrapper` makes the specifies the number of iterations to run at\ntraining and inference.\n\nIn conclusion, your script should be similar to this:\n\n```python\ndataset = ActiveLearningDataset(your_dataset)\ndataset.label_randomly(INITIAL_POOL)  # label some data\nmodel = MCDropoutModule(your_model)\nmodel = ModelWrapper(model, your_criterion)\nactive_loop = ActiveLearningLoop(dataset,\n                                 get_probabilities=model.predict_on_dataset,\n                                 heuristic=heuristics.BALD(shuffle_prop=0.1),\n                                 query_size=NDATA_TO_LABEL)\nfor al_step in range(N_ALSTEP):\n    model.train_on_dataset(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda)\n    if not active_loop.step():\n        # We\'re done!\n        break\n```\n\nFor a complete experiment, we provide _[experiments/](experiments/)_ to understand how to write an active training\nprocess. Generally, we use the **ActiveLearningLoop**\nprovided at _[src/baal/active/active_loop.py](baal/active/active_loop.py)_. This class provides functionality to get the\npredictions on the unlabeled pool after each (few) epoch(s) and sort the next set of data items to be labeled based on\nthe calculated uncertainty of the pool.\n\n### Re-run our Experiments\n\n```bash\ndocker build [--target base_baal] -t baal .\ndocker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py \n```\n\n### Use Baal for YOUR Experiments\n\nSimply clone the repo, and create your own experiment script similar to the example\nat [experiments/vgg_experiment.py](experiments/vgg_experiment.py). Make sure to use the four main parts of Baal\nframework. _Happy running experiments_\n\n### Contributing!\n\nTo contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md).\n\n### Who We Are!\n\n"There is passion, yet peace; serenity, yet emotion; chaos, yet order."\n\nThe Baal team tests and implements the most recent papers on uncertainty estimation and active learning.\n\nCurrent maintainers:\n\n- [Parmida Atighehchian](mailto:patighehchian@twitter.com)\n- [Frédéric Branchaud-Charron](mailto:frederic.branchaud-charron@gmail.com)\n- [George Pearse](georgehwp26@gmail.com)\n\n### How to cite\n\nIf you used Baal in one of your project, we would greatly appreciate if you cite this library using this Bibtex:\n\n```\n@misc{atighehchian2019baal,\n  title={Baal, a bayesian active learning library},\n  author={Atighehchian, Parmida and Branchaud-Charron, Frederic and Freyberg, Jan and Pardinas, Rafael and Schell, Lorne\n          and Pearse, George},\n  year={2022},\n  howpublished={\\url{https://github.com/baal-org/baal/}},\n}\n```\n\n### Licence\n\nTo get information on licence of this API please read [LICENCE](./LICENSE)\n',
+    'long_description': '<p align="center">\n  <img height=15% width=25% src="https://i.imgur.com/Zdzb2QZ.png" style="max-width: 100%;border-radius: 25%;">\n  <h1 align="center">Bayesian Active Learning (Baal)\n   <br>\n  <a href="https://github.com/baal-org/baal/actions/workflows/pythonci.yml">\n    <img alt="Python CI" src="https://github.com/baal-org/baal/actions/workflows/pythonci.yml/badge.svg"/>\n  </a>\n  <a href="https://baal.readthedocs.io/en/latest/?badge=latest">\n    <img alt="Documentation Status" src="https://readthedocs.org/projects/baal/badge/?version=latest"/>\n  </a>\n  <a href="https://join.slack.com/t/baal-world/shared_invite/zt-z0izhn4y-Jt6Zu5dZaV2rsAS9sdISfg">\n    <img alt="Slack" src="https://img.shields.io/badge/slack-chat-green.svg?logo=slack"/>\n  </a>\n  <a href="https://github.com/Elementai/baal/blob/master/LICENSE">\n    <img alt="Licence" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/>\n  </a>\n  <a href="https://calendly.com/baal-org/30min">\n    <img alt="Office hours" src="https://img.shields.io/badge/Office hours-Calendly-blue.svg"/>\n  </a>\n  <a href="https://pepy.tech/project/baal">\n    <img alt="Downloads" src="https://pepy.tech/badge/baal"/>\n  </a>\n\n  </h1>\n</p>\n\nBaal is an active learning library that supports both industrial applications and research usecases.\n\nRead the documentation at https://baal.readthedocs.io.\n\nOur paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes tips and tricks to make active learning\nusable in production.\n\nFor a quick introduction to Baal and Bayesian active learning, please see these links:\n\n- [Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)\n- [User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)\n- [Bayesian active learning presentation](https://drive.google.com/file/d/13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)\n\n*Baal was initially developed at [ElementAI](https://www.elementai.com/) (acquired by ServiceNow in 2021), but is now independant.*\n\n\n## Installation and requirements\n\nBaal requires `Python>=3.8`.\n\nTo install Baal using pip: `pip install baal`\n\nWe use [Poetry](https://python-poetry.org/) as our package manager.\nTo install Baal from source: `poetry install`\n\n## Papers using Baal\n\n- [Bayesian active learning for production, a systematic study and a reusable library\n  ](https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020)\n- [Synbols: Probing Learning Algorithms with Synthetic Datasets\n  ](https://nips.cc/virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020)\n- [Can Active Learning Preemptively Mitigate Fairness Issues?\n  ](https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)\n- [Active learning with MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/2112.06586) (\n  Blok et al. 2021)\n- [Stochastic Batch Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)\n\n# What is active learning?\n\nActive learning is a special case of machine learning in which a learning algorithm is able to interactively query the\nuser (or some other information source) to obtain the desired outputs at new data points\n(to understand the concept in more depth, refer to our [tutorial](https://baal.readthedocs.io/en/latest/)).\n\n## Baal Framework\n\nAt the moment Baal supports the following methods to perform active learning.\n\n- Monte-Carlo Dropout (Gal et al. 2015)\n- MCDropConnect (Mobiny et al. 2019)\n- Deep ensembles\n- Semi-supervised learning\n\nIf you want to propose new methods, please submit an issue.\n\nThe **Monte-Carlo Dropout** method is a known approximation for Bayesian neural networks. In this method, the Dropout\nlayer is used both in training and test time. By running the model multiple times whilst randomly dropping weights, we\ncalculate the uncertainty of the prediction using one of the uncertainty measurements\nin [heuristics.py](baal/active/heuristics/heuristics.py).\n\nThe framework consists of four main parts, as demonstrated in the flowchart below:\n\n- ActiveLearningDataset\n- Heuristics\n- ModelWrapper\n- ActiveLearningLoop\n\n<p align="center">\n  <img src="docs/research/literature/images/Baalscheme.svg">\n</p>\n\nTo get started, wrap your dataset in our _[**ActiveLearningDataset**](baal/active/dataset.py)_ class. This will ensure\nthat the dataset is split into\n`training` and `pool` sets. The `pool` set represents the portion of the training set which is yet to be labelled.\n\nWe provide a lightweight object _[**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it easier to\ntrain and test the model. If your model is not ready for active learning, we provide Modules to prepare them.\n\nFor example, the _[**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing dropout layer to be used\nin both training and inference time and the `ModelWrapper` makes the specifies the number of iterations to run at\ntraining and inference.\n\nFinally, _[**ActiveLearningLoop**](baal/active/active_loop.py)_ automatically computes the uncertainty and label the most\nuncertain items in the pool.\n\nIn conclusion, your script should be similar to this:\n\n```python\ndataset = ActiveLearningDataset(your_dataset)\ndataset.label_randomly(INITIAL_POOL)  # label some data\nmodel = MCDropoutModule(your_model)\nmodel = ModelWrapper(model, your_criterion)\nactive_loop = ActiveLearningLoop(dataset,\n                                 get_probabilities=model.predict_on_dataset,\n                                 heuristic=heuristics.BALD(),\n                                 iterations=20, # Number of MC sampling.\n                                 query_size=QUERY_SIZE)  # Number of item to label.\nfor al_step in range(N_ALSTEP):\n    model.train_on_dataset(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda)\n    metrics = model.test_on_dataset(test_dataset, BATCH_SIZE)\n    # Label the next most uncertain items.\n    if not active_loop.step():\n        # We\'re done!\n        break\n```\n\nFor a complete experiment, see _[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_ .\n\n### Re-run our Experiments\n\n```bash\ndocker build [--target base_baal] -t baal .\ndocker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py\n```\n\n### Use Baal for YOUR Experiments\n\nSimply clone the repo, and create your own experiment script similar to the example\nat _[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_. Make sure to use the four main parts of Baal\nframework. _Happy running experiments_\n\n### Contributing!\n\nTo contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md).\n\n### Who We Are!\n\n"There is passion, yet peace; serenity, yet emotion; chaos, yet order."\n\nThe Baal team tests and implements the most recent papers on uncertainty estimation and active learning.\n\nCurrent maintainers:\n\n- [Parmida Atighehchian](mailto:patighehchian@twitter.com)\n- [Frédéric Branchaud-Charron](mailto:frederic.branchaud-charron@gmail.com)\n- [George Pearse](georgehwp26@gmail.com)\n\n### How to cite\n\nIf you used Baal in one of your project, we would greatly appreciate if you cite this library using this Bibtex:\n\n```\n@misc{atighehchian2019baal,\n  title={Baal, a bayesian active learning library},\n  author={Atighehchian, Parmida and Branchaud-Charron, Frederic and Freyberg, Jan and Pardinas, Rafael and Schell, Lorne\n          and Pearse, George},\n  year={2022},\n  howpublished={\\url{https://github.com/baal-org/baal/}},\n}\n```\n\n### Licence\n\nTo get information on licence of this API please read [LICENCE](./LICENSE)\n',
     'author': 'Parmida Atighehchian',
     'author_email': 'parmida.atighehchian@servicenow.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ElementAI/baal/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,106 +1,105 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['baal',
 'baal.active', 'baal.active.dataset', 'baal.active.heuristics',
 'baal.bayesian', 'baal.calibration', 'baal.metrics', 'baal.utils'] package_data
 = \ {'': ['*']} install_requires = \ ['Pillow>=6.2.0', 'h5py>=3.4.0,<4.0.0',
 'matplotlib>=3.4.3,<4.0.0', 'numpy>=1.21.2,<2.0.0', 'scikit-
 learn>=1.0.0,<2.0.0', 'scipy>=1.7.1,<2.0.0', 'structlog>=21.1.0,<22.0.0',
 'torch>=1.6.0', 'torchmetrics>=0.9.3,<0.10.0', 'tqdm>=4.62.2,<5.0.0']
-extras_require = \ {'nlp': ['transformers>=4.10.2,<5.0.0',
-'datasets>=1.11.0,<2.0.0'], 'vision': ['torchvision>=0.7.0', 'lightning-
-flash>=0.7.5,<0.8.0']} setup_kwargs = { 'name': 'baal', 'version': '1.7.0',
-'description': 'Library to enable Bayesian active learning in your research or
-labeling work.', 'long_description': '
-  \n [https://github.com/ElementAI/baal/blob/master/docs/_static/images/logo-
-                         with-bg-solid.png?raw=true]\n
+extras_require = \ {'nlp': ['transformers>=4.10.2', 'datasets>=1.11.0'],
+'vision': ['torchvision>=0.7.0', 'lightning-flash>=0.7.5']} setup_kwargs =
+{ 'name': 'baal', 'version': '1.8.0', 'description': 'Library to enable
+Bayesian active learning in your research or labeling work.',
+'long_description': '
+                    \n [https://i.imgur.com/Zdzb2QZ.png]\n
                    ****** Bayesian Active Learning (Baal)\n
     \n \n_[Python_CI]\n\n \n_[Documentation_Status]\n\n \n_[Slack]\n\n \n_
         [Licence]\n\n \n_[Office_hours]\n\n \n_[Downloads]\n\n\n ******
 \n
-\n\n\nBaal is an active learning library initially developed at\n[ElementAI]
-(https://www.elementai.com/) (acquired by ServiceNow in 2021).\n\nOur goal is
-to support both industrial applications and research in active
-learning.\n\nRead the documentation at https://baal.readthedocs.io.\n\nOur
-paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes
-tips and tricks to make active learning\nusable in production.\n\nFor a quick
-introduction to Baal and Bayesian active learning, please see these links:\n\n*
-[Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)\n*
-[User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)\n*
-[Bayesian active learning presentation](https://drive.google.com/file/d/
-13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)\n\n## Installation and
-requirements\n\nBaal requires `Python>=3.7`.\n\nTo install Baal using pip: `pip
-install baal`\n\nWe use [Poetry](https://python-poetry.org/) as our package
-manager.\nTo install Baal from source: `poetry install`\n\n## Papers using
-Baal\n\n* [Bayesian active learning for production, a systematic study and a
-reusable library\n ](https://arxiv.org/abs/2006.09916) (Atighehchian et al.
-2020)\n* [Synbols: Probing Learning Algorithms with Synthetic Datasets\n ]
-(https://nips.cc/virtual/2020/public/
-poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020)\n* [Can
-Active Learning Preemptively Mitigate Fairness Issues?\n ](https://arxiv.org/
-pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)\n* [Active learning with
-MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/
-abs/2112.06586) (\n Blok et al. 2021)\n* [Stochastic Batch Acquisition for Deep
-Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)\n\n#
-What is active learning?\n\nActive learning is a special case of machine
-learning in which a learning algorithm is able to interactively query the\nuser
-(or some other information source) to obtain the desired outputs at new data
-points\n(to understand the concept in more depth, refer to our [tutorial]
-(https://baal.readthedocs.io/en/latest/)).\n\n## Baal Framework\n\nAt the
-moment Baal supports the following methods to perform active learning.\n\n-
-Monte-Carlo Dropout (Gal et al. 2015)\n- MCDropConnect (Mobiny et al. 2019)\n-
-Deep ensembles\n- Semi-supervised learning\n\nIf you want to propose new
-methods, please submit an issue.\n\nThe **Monte-Carlo Dropout** method is a
-known approximation for Bayesian neural networks. In this method, the
-Dropout\nlayer is used both in training and test time. By running the model
-multiple times whilst randomly dropping weights, we\ncalculate the uncertainty
-of the prediction using one of the uncertainty measurements\nin [heuristics.py]
-(baal/active/heuristics/heuristics.py).\n\nThe framework consists of four main
-parts, as demonstrated in the flowchart below:\n\n- ActiveLearningDataset\n-
-Heuristics\n- ModelWrapper\n- ActiveLearningLoop\n\n
+\n\nBaal is an active learning library that supports both industrial
+applications and research usecases.\n\nRead the documentation at https://
+baal.readthedocs.io.\n\nOur paper can be read on [arXiv](https://arxiv.org/abs/
+2006.09916). It includes tips and tricks to make active learning\nusable in
+production.\n\nFor a quick introduction to Baal and Bayesian active learning,
+please see these links:\n\n- [Seminar with Label Studio](https://
+www.youtube.com/watch?v=HG7imRQN3-k)\n- [User guide](https://
+baal.readthedocs.io/en/latest/user_guide/index.html)\n- [Bayesian active
+learning presentation](https://drive.google.com/file/d/
+13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)\n\n*Baal was initially
+developed at [ElementAI](https://www.elementai.com/) (acquired by ServiceNow in
+2021), but is now independant.*\n\n\n## Installation and requirements\n\nBaal
+requires `Python>=3.8`.\n\nTo install Baal using pip: `pip install baal`\n\nWe
+use [Poetry](https://python-poetry.org/) as our package manager.\nTo install
+Baal from source: `poetry install`\n\n## Papers using Baal\n\n- [Bayesian
+active learning for production, a systematic study and a reusable library\n ]
+(https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020)\n- [Synbols:
+Probing Learning Algorithms with Synthetic Datasets\n ](https://nips.cc/
+virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et
+al. 2020)\n- [Can Active Learning Preemptively Mitigate Fairness Issues?\n ]
+(https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)\n-
+[Active learning with MaskAL reduces annotation effort for training Mask R-CNN]
+(https://arxiv.org/abs/2112.06586) (\n Blok et al. 2021)\n- [Stochastic Batch
+Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch
+et al. 2022)\n\n# What is active learning?\n\nActive learning is a special case
+of machine learning in which a learning algorithm is able to interactively
+query the\nuser (or some other information source) to obtain the desired
+outputs at new data points\n(to understand the concept in more depth, refer to
+our [tutorial](https://baal.readthedocs.io/en/latest/)).\n\n## Baal
+Framework\n\nAt the moment Baal supports the following methods to perform
+active learning.\n\n- Monte-Carlo Dropout (Gal et al. 2015)\n- MCDropConnect
+(Mobiny et al. 2019)\n- Deep ensembles\n- Semi-supervised learning\n\nIf you
+want to propose new methods, please submit an issue.\n\nThe **Monte-Carlo
+Dropout** method is a known approximation for Bayesian neural networks. In this
+method, the Dropout\nlayer is used both in training and test time. By running
+the model multiple times whilst randomly dropping weights, we\ncalculate the
+uncertainty of the prediction using one of the uncertainty measurements\nin
+[heuristics.py](baal/active/heuristics/heuristics.py).\n\nThe framework
+consists of four main parts, as demonstrated in the flowchart below:\n\n-
+ActiveLearningDataset\n- Heuristics\n- ModelWrapper\n- ActiveLearningLoop\n\n
              \n [docs/research/literature/images/Baalscheme.svg]\n
 \n\nTo get started, wrap your dataset in our _[**ActiveLearningDataset**](baal/
 active/dataset.py)_ class. This will ensure\nthat the dataset is split
 into\n`training` and `pool` sets. The `pool` set represents the portion of the
 training set which is yet to be labelled.\n\nWe provide a lightweight object _
 [**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it
 easier to\ntrain and test the model. If your model is not ready for active
 learning, we provide Modules to prepare them.\n\nFor example, the _
 [**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing
 dropout layer to be used\nin both training and inference time and the
 `ModelWrapper` makes the specifies the number of iterations to run at\ntraining
-and inference.\n\nIn conclusion, your script should be similar to this:
-\n\n```python\ndataset = ActiveLearningDataset
+and inference.\n\nFinally, _[**ActiveLearningLoop**](baal/active/
+active_loop.py)_ automatically computes the uncertainty and label the
+most\nuncertain items in the pool.\n\nIn conclusion, your script should be
+similar to this:\n\n```python\ndataset = ActiveLearningDataset
 (your_dataset)\ndataset.label_randomly(INITIAL_POOL) # label some data\nmodel =
 MCDropoutModule(your_model)\nmodel = ModelWrapper(model,
 your_criterion)\nactive_loop = ActiveLearningLoop(dataset,\n
-get_probabilities=model.predict_on_dataset,\n heuristic=heuristics.BALD
-(shuffle_prop=0.1),\n query_size=NDATA_TO_LABEL)\nfor al_step in range
-(N_ALSTEP):\n model.train_on_dataset(dataset, optimizer, BATCH_SIZE,
-use_cuda=use_cuda)\n if not active_loop.step():\n # We\'re done!\n
-break\n```\n\nFor a complete experiment, we provide _[experiments/]
-(experiments/)_ to understand how to write an active training\nprocess.
-Generally, we use the **ActiveLearningLoop**\nprovided at _[src/baal/active/
-active_loop.py](baal/active/active_loop.py)_. This class provides functionality
-to get the\npredictions on the unlabeled pool after each (few) epoch(s) and
-sort the next set of data items to be labeled based on\nthe calculated
-uncertainty of the pool.\n\n### Re-run our Experiments\n\n```bash\ndocker build
-[--target base_baal] -t baal .\ndocker run --rm baal --gpus all python3
-experiments/vgg_mcdropout_cifar10.py \n```\n\n### Use Baal for YOUR
-Experiments\n\nSimply clone the repo, and create your own experiment script
-similar to the example\nat [experiments/vgg_experiment.py](experiments/
-vgg_experiment.py). Make sure to use the four main parts of Baal\nframework.
-_Happy running experiments_\n\n### Contributing!\n\nTo contribute, see
-[CONTRIBUTING.md](./CONTRIBUTING.md).\n\n### Who We Are!\n\n"There is passion,
-yet peace; serenity, yet emotion; chaos, yet order."\n\nThe Baal team tests and
-implements the most recent papers on uncertainty estimation and active
-learning.\n\nCurrent maintainers:\n\n- [Parmida Atighehchian](mailto:
-patighehchian@twitter.com)\n- [FrÃ©dÃ©ric Branchaud-Charron](mailto:
-frederic.branchaud-charron@gmail.com)\n- [George Pearse]
-(georgehwp26@gmail.com)\n\n### How to cite\n\nIf you used Baal in one of your
-project, we would greatly appreciate if you cite this library using this
+get_probabilities=model.predict_on_dataset,\n heuristic=heuristics.BALD(),\n
+iterations=20, # Number of MC sampling.\n query_size=QUERY_SIZE) # Number of
+item to label.\nfor al_step in range(N_ALSTEP):\n model.train_on_dataset
+(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda)\n metrics =
+model.test_on_dataset(test_dataset, BATCH_SIZE)\n # Label the next most
+uncertain items.\n if not active_loop.step():\n # We\'re done!\n
+break\n```\n\nFor a complete experiment, see _[experiments/
+vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_ .\n\n### Re-
+run our Experiments\n\n```bash\ndocker build [--target base_baal] -t baal
+.\ndocker run --rm baal --gpus all python3 experiments/
+vgg_mcdropout_cifar10.py\n```\n\n### Use Baal for YOUR Experiments\n\nSimply
+clone the repo, and create your own experiment script similar to the
+example\nat _[experiments/vgg_mcdropout_cifar10.py](experiments/
+vgg_mcdropout_cifar10.py)_. Make sure to use the four main parts of
+Baal\nframework. _Happy running experiments_\n\n### Contributing!\n\nTo
+contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md).\n\n### Who We
+Are!\n\n"There is passion, yet peace; serenity, yet emotion; chaos, yet
+order."\n\nThe Baal team tests and implements the most recent papers on
+uncertainty estimation and active learning.\n\nCurrent maintainers:\n\n-
+[Parmida Atighehchian](mailto:patighehchian@twitter.com)\n- [FrÃ©dÃ©ric
+Branchaud-Charron](mailto:frederic.branchaud-charron@gmail.com)\n- [George
+Pearse](georgehwp26@gmail.com)\n\n### How to cite\n\nIf you used Baal in one of
+your project, we would greatly appreciate if you cite this library using this
 Bibtex:\n\n```\n@misc{atighehchian2019baal,\n title={Baal, a bayesian active
 learning library},\n author={Atighehchian, Parmida and Branchaud-Charron,
 Frederic and Freyberg, Jan and Pardinas, Rafael and Schell, Lorne\n and Pearse,
 George},\n year={2022},\n howpublished={\\url{https://github.com/baal-org/baal/
 }},\n}\n```\n\n### Licence\n\nTo get information on licence of this API please
 read [LICENCE](./LICENSE)\n', 'author': 'Parmida Atighehchian', 'author_email':
 'parmida.atighehchian@servicenow.com', 'maintainer': None, 'maintainer_email':
```

### Comparing `baal-1.7.0/PKG-INFO` & `baal-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: baal
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library to enable Bayesian active learning in your research or labeling work.
 Home-page: https://github.com/ElementAI/baal/
 License: Apache-2.0
 Author: Parmida Atighehchian
 Author-email: parmida.atighehchian@servicenow.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: nlp
 Provides-Extra: vision
 Requires-Dist: Pillow (>=6.2.0)
-Requires-Dist: datasets (>=1.11.0,<2.0.0); extra == "nlp"
+Requires-Dist: datasets (>=1.11.0); extra == "nlp"
 Requires-Dist: h5py (>=3.4.0,<4.0.0)
-Requires-Dist: lightning-flash (>=0.7.5,<0.8.0); extra == "vision"
+Requires-Dist: lightning-flash (>=0.7.5); extra == "vision"
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: structlog (>=21.1.0,<22.0.0)
 Requires-Dist: torch (>=1.6.0)
 Requires-Dist: torchmetrics (>=0.9.3,<0.10.0)
 Requires-Dist: torchvision (>=0.7.0); extra == "vision"
 Requires-Dist: tqdm (>=4.62.2,<5.0.0)
-Requires-Dist: transformers (>=4.10.2,<5.0.0); extra == "nlp"
+Requires-Dist: transformers (>=4.10.2); extra == "nlp"
 Project-URL: Documentation, https://baal.readthedocs.io
 Project-URL: Repository, https://github.com/ElementAI/baal/
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img height=15% width=25% src="https://github.com/ElementAI/baal/blob/master/docs/_static/images/logo-with-bg-solid.png?raw=true">
+  <img height=15% width=25% src="https://i.imgur.com/Zdzb2QZ.png" style="max-width: 100%;border-radius: 25%;">
   <h1 align="center">Bayesian Active Learning (Baal)
    <br>
   <a href="https://github.com/baal-org/baal/actions/workflows/pythonci.yml">
     <img alt="Python CI" src="https://github.com/baal-org/baal/actions/workflows/pythonci.yml/badge.svg"/>
   </a>
   <a href="https://baal.readthedocs.io/en/latest/?badge=latest">
     <img alt="Documentation Status" src="https://readthedocs.org/projects/baal/badge/?version=latest"/>
@@ -54,51 +54,50 @@
   <a href="https://pepy.tech/project/baal">
     <img alt="Downloads" src="https://pepy.tech/badge/baal"/>
   </a>
 
   </h1>
 </p>
 
-
-Baal is an active learning library initially developed at
-[ElementAI](https://www.elementai.com/) (acquired by ServiceNow in 2021).
-
-Our goal is to support both industrial applications and research in active learning.
+Baal is an active learning library that supports both industrial applications and research usecases.
 
 Read the documentation at https://baal.readthedocs.io.
 
 Our paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes tips and tricks to make active learning
 usable in production.
 
 For a quick introduction to Baal and Bayesian active learning, please see these links:
 
-* [Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)
-* [User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)
-* [Bayesian active learning presentation](https://drive.google.com/file/d/13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)
+- [Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k)
+- [User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html)
+- [Bayesian active learning presentation](https://drive.google.com/file/d/13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing)
+
+*Baal was initially developed at [ElementAI](https://www.elementai.com/) (acquired by ServiceNow in 2021), but is now independant.*
+
 
 ## Installation and requirements
 
-Baal requires `Python>=3.7`.
+Baal requires `Python>=3.8`.
 
 To install Baal using pip: `pip install baal`
 
 We use [Poetry](https://python-poetry.org/) as our package manager.
 To install Baal from source: `poetry install`
 
 ## Papers using Baal
 
-* [Bayesian active learning for production, a systematic study and a reusable library
+- [Bayesian active learning for production, a systematic study and a reusable library
   ](https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020)
-* [Synbols: Probing Learning Algorithms with Synthetic Datasets
+- [Synbols: Probing Learning Algorithms with Synthetic Datasets
   ](https://nips.cc/virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020)
-* [Can Active Learning Preemptively Mitigate Fairness Issues?
+- [Can Active Learning Preemptively Mitigate Fairness Issues?
   ](https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)
-* [Active learning with MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/2112.06586) (
+- [Active learning with MaskAL reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/2112.06586) (
   Blok et al. 2021)
-* [Stochastic Batch Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)
+- [Stochastic Batch Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022)
 
 # What is active learning?
 
 Active learning is a special case of machine learning in which a learning algorithm is able to interactively query the
 user (or some other information source) to obtain the desired outputs at new data points
 (to understand the concept in more depth, refer to our [tutorial](https://baal.readthedocs.io/en/latest/)).
 
@@ -136,49 +135,51 @@
 We provide a lightweight object _[**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it easier to
 train and test the model. If your model is not ready for active learning, we provide Modules to prepare them.
 
 For example, the _[**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing dropout layer to be used
 in both training and inference time and the `ModelWrapper` makes the specifies the number of iterations to run at
 training and inference.
 
+Finally, _[**ActiveLearningLoop**](baal/active/active_loop.py)_ automatically computes the uncertainty and label the most
+uncertain items in the pool.
+
 In conclusion, your script should be similar to this:
 
 ```python
 dataset = ActiveLearningDataset(your_dataset)
 dataset.label_randomly(INITIAL_POOL)  # label some data
 model = MCDropoutModule(your_model)
 model = ModelWrapper(model, your_criterion)
 active_loop = ActiveLearningLoop(dataset,
                                  get_probabilities=model.predict_on_dataset,
-                                 heuristic=heuristics.BALD(shuffle_prop=0.1),
-                                 query_size=NDATA_TO_LABEL)
+                                 heuristic=heuristics.BALD(),
+                                 iterations=20, # Number of MC sampling.
+                                 query_size=QUERY_SIZE)  # Number of item to label.
 for al_step in range(N_ALSTEP):
     model.train_on_dataset(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda)
+    metrics = model.test_on_dataset(test_dataset, BATCH_SIZE)
+    # Label the next most uncertain items.
     if not active_loop.step():
         # We're done!
         break
 ```
 
-For a complete experiment, we provide _[experiments/](experiments/)_ to understand how to write an active training
-process. Generally, we use the **ActiveLearningLoop**
-provided at _[src/baal/active/active_loop.py](baal/active/active_loop.py)_. This class provides functionality to get the
-predictions on the unlabeled pool after each (few) epoch(s) and sort the next set of data items to be labeled based on
-the calculated uncertainty of the pool.
+For a complete experiment, see _[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_ .
 
 ### Re-run our Experiments
 
 ```bash
 docker build [--target base_baal] -t baal .
-docker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py 
+docker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py
 ```
 
 ### Use Baal for YOUR Experiments
 
 Simply clone the repo, and create your own experiment script similar to the example
-at [experiments/vgg_experiment.py](experiments/vgg_experiment.py). Make sure to use the four main parts of Baal
+at _[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_. Make sure to use the four main parts of Baal
 framework. _Happy running experiments_
 
 ### Contributing!
 
 To contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md).
 
 ### Who We Are!
```

#### html2text {}

```diff
@@ -1,107 +1,104 @@
-Metadata-Version: 2.1 Name: baal Version: 1.7.0 Summary: Library to enable
+Metadata-Version: 2.1 Name: baal Version: 1.8.0 Summary: Library to enable
 Bayesian active learning in your research or labeling work. Home-page: https://
 github.com/ElementAI/baal/ License: Apache-2.0 Author: Parmida Atighehchian
 Author-email: parmida.atighehchian@servicenow.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Provides-Extra: nlp Provides-Extra:
-vision Requires-Dist: Pillow (>=6.2.0) Requires-Dist: datasets
-(>=1.11.0,<2.0.0); extra == "nlp" Requires-Dist: h5py (>=3.4.0,<4.0.0)
-Requires-Dist: lightning-flash (>=0.7.5,<0.8.0); extra == "vision" Requires-
-Dist: matplotlib (>=3.4.3,<4.0.0) Requires-Dist: numpy (>=1.21.2,<2.0.0)
-Requires-Dist: scikit-learn (>=1.0.0,<2.0.0) Requires-Dist: scipy
-(>=1.7.1,<2.0.0) Requires-Dist: structlog (>=21.1.0,<22.0.0) Requires-Dist:
-torch (>=1.6.0) Requires-Dist: torchmetrics (>=0.9.3,<0.10.0) Requires-Dist:
-torchvision (>=0.7.0); extra == "vision" Requires-Dist: tqdm (>=4.62.2,<5.0.0)
-Requires-Dist: transformers (>=4.10.2,<5.0.0); extra == "nlp" Project-URL:
-Documentation, https://baal.readthedocs.io Project-URL: Repository, https://
-github.com/ElementAI/baal/ Description-Content-Type: text/markdown
- [https://github.com/ElementAI/baal/blob/master/docs/_static/images/logo-with-
-                            bg-solid.png?raw=true]
+vision Requires-Dist: Pillow (>=6.2.0) Requires-Dist: datasets (>=1.11.0);
+extra == "nlp" Requires-Dist: h5py (>=3.4.0,<4.0.0) Requires-Dist: lightning-
+flash (>=0.7.5); extra == "vision" Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
+Requires-Dist: numpy (>=1.21.2,<2.0.0) Requires-Dist: scikit-learn
+(>=1.0.0,<2.0.0) Requires-Dist: scipy (>=1.7.1,<2.0.0) Requires-Dist: structlog
+(>=21.1.0,<22.0.0) Requires-Dist: torch (>=1.6.0) Requires-Dist: torchmetrics
+(>=0.9.3,<0.10.0) Requires-Dist: torchvision (>=0.7.0); extra == "vision"
+Requires-Dist: tqdm (>=4.62.2,<5.0.0) Requires-Dist: transformers (>=4.10.2);
+extra == "nlp" Project-URL: Documentation, https://baal.readthedocs.io Project-
+URL: Repository, https://github.com/ElementAI/baal/ Description-Content-Type:
+text/markdown
+                       [https://i.imgur.com/Zdzb2QZ.png]
                     ****** Bayesian Active Learning (Baal)
 [Python_CI] [Documentation_Status] [Slack] [Licence] [Office_hours] [Downloads]
                                     ******
-Baal is an active learning library initially developed at [ElementAI](https://
-www.elementai.com/) (acquired by ServiceNow in 2021). Our goal is to support
-both industrial applications and research in active learning. Read the
-documentation at https://baal.readthedocs.io. Our paper can be read on [arXiv]
-(https://arxiv.org/abs/2006.09916). It includes tips and tricks to make active
-learning usable in production. For a quick introduction to Baal and Bayesian
-active learning, please see these links: * [Seminar with Label Studio](https://
-www.youtube.com/watch?v=HG7imRQN3-k) * [User guide](https://
-baal.readthedocs.io/en/latest/user_guide/index.html) * [Bayesian active
-learning presentation](https://drive.google.com/file/d/
-13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing) ## Installation and
-requirements Baal requires `Python>=3.7`. To install Baal using pip: `pip
-install baal` We use [Poetry](https://python-poetry.org/) as our package
-manager. To install Baal from source: `poetry install` ## Papers using Baal *
-[Bayesian active learning for production, a systematic study and a reusable
-library ](https://arxiv.org/abs/2006.09916) (Atighehchian et al. 2020) *
-[Synbols: Probing Learning Algorithms with Synthetic Datasets ](https://
-nips.cc/virtual/2020/public/poster_0169cf885f882efd795951253db5cdfb.html)
-(Lacoste et al. 2020) * [Can Active Learning Preemptively Mitigate Fairness
-Issues? ](https://arxiv.org/pdf/2104.06879.pdf) (Branchaud-Charron et al. 2021)
-* [Active learning with MaskAL reduces annotation effort for training Mask R-
-CNN](https://arxiv.org/abs/2112.06586) ( Blok et al. 2021) * [Stochastic Batch
-Acquisition for Deep Active Learning](https://arxiv.org/abs/2106.12059) (Kirsch
-et al. 2022) # What is active learning? Active learning is a special case of
-machine learning in which a learning algorithm is able to interactively query
-the user (or some other information source) to obtain the desired outputs at
-new data points (to understand the concept in more depth, refer to our
-[tutorial](https://baal.readthedocs.io/en/latest/)). ## Baal Framework At the
-moment Baal supports the following methods to perform active learning. - Monte-
-Carlo Dropout (Gal et al. 2015) - MCDropConnect (Mobiny et al. 2019) - Deep
-ensembles - Semi-supervised learning If you want to propose new methods, please
-submit an issue. The **Monte-Carlo Dropout** method is a known approximation
-for Bayesian neural networks. In this method, the Dropout layer is used both in
-training and test time. By running the model multiple times whilst randomly
-dropping weights, we calculate the uncertainty of the prediction using one of
-the uncertainty measurements in [heuristics.py](baal/active/heuristics/
-heuristics.py). The framework consists of four main parts, as demonstrated in
-the flowchart below: - ActiveLearningDataset - Heuristics - ModelWrapper -
-ActiveLearningLoop
+Baal is an active learning library that supports both industrial applications
+and research usecases. Read the documentation at https://baal.readthedocs.io.
+Our paper can be read on [arXiv](https://arxiv.org/abs/2006.09916). It includes
+tips and tricks to make active learning usable in production. For a quick
+introduction to Baal and Bayesian active learning, please see these links: -
+[Seminar with Label Studio](https://www.youtube.com/watch?v=HG7imRQN3-k) -
+[User guide](https://baal.readthedocs.io/en/latest/user_guide/index.html) -
+[Bayesian active learning presentation](https://drive.google.com/file/d/
+13UUDsS1rvqDnXza7L0j4bnqyhOT5TDSt/view?usp=sharing) *Baal was initially
+developed at [ElementAI](https://www.elementai.com/) (acquired by ServiceNow in
+2021), but is now independant.* ## Installation and requirements Baal requires
+`Python>=3.8`. To install Baal using pip: `pip install baal` We use [Poetry]
+(https://python-poetry.org/) as our package manager. To install Baal from
+source: `poetry install` ## Papers using Baal - [Bayesian active learning for
+production, a systematic study and a reusable library ](https://arxiv.org/abs/
+2006.09916) (Atighehchian et al. 2020) - [Synbols: Probing Learning Algorithms
+with Synthetic Datasets ](https://nips.cc/virtual/2020/public/
+poster_0169cf885f882efd795951253db5cdfb.html) (Lacoste et al. 2020) - [Can
+Active Learning Preemptively Mitigate Fairness Issues? ](https://arxiv.org/pdf/
+2104.06879.pdf) (Branchaud-Charron et al. 2021) - [Active learning with MaskAL
+reduces annotation effort for training Mask R-CNN](https://arxiv.org/abs/
+2112.06586) ( Blok et al. 2021) - [Stochastic Batch Acquisition for Deep Active
+Learning](https://arxiv.org/abs/2106.12059) (Kirsch et al. 2022) # What is
+active learning? Active learning is a special case of machine learning in which
+a learning algorithm is able to interactively query the user (or some other
+information source) to obtain the desired outputs at new data points (to
+understand the concept in more depth, refer to our [tutorial](https://
+baal.readthedocs.io/en/latest/)). ## Baal Framework At the moment Baal supports
+the following methods to perform active learning. - Monte-Carlo Dropout (Gal et
+al. 2015) - MCDropConnect (Mobiny et al. 2019) - Deep ensembles - Semi-
+supervised learning If you want to propose new methods, please submit an issue.
+The **Monte-Carlo Dropout** method is a known approximation for Bayesian neural
+networks. In this method, the Dropout layer is used both in training and test
+time. By running the model multiple times whilst randomly dropping weights, we
+calculate the uncertainty of the prediction using one of the uncertainty
+measurements in [heuristics.py](baal/active/heuristics/heuristics.py). The
+framework consists of four main parts, as demonstrated in the flowchart below:
+- ActiveLearningDataset - Heuristics - ModelWrapper - ActiveLearningLoop
                [docs/research/literature/images/Baalscheme.svg]
 To get started, wrap your dataset in our _[**ActiveLearningDataset**](baal/
 active/dataset.py)_ class. This will ensure that the dataset is split into
 `training` and `pool` sets. The `pool` set represents the portion of the
 training set which is yet to be labelled. We provide a lightweight object _
 [**ModelWrapper**](baal/modelwrapper.py)_ similar to `keras.Model` to make it
 easier to train and test the model. If your model is not ready for active
 learning, we provide Modules to prepare them. For example, the _
 [**MCDropoutModule**](baal/bayesian/dropout.py)_ wrapper changes the existing
 dropout layer to be used in both training and inference time and the
 `ModelWrapper` makes the specifies the number of iterations to run at training
-and inference. In conclusion, your script should be similar to this: ```python
+and inference. Finally, _[**ActiveLearningLoop**](baal/active/active_loop.py)_
+automatically computes the uncertainty and label the most uncertain items in
+the pool. In conclusion, your script should be similar to this: ```python
 dataset = ActiveLearningDataset(your_dataset) dataset.label_randomly
 (INITIAL_POOL) # label some data model = MCDropoutModule(your_model) model =
 ModelWrapper(model, your_criterion) active_loop = ActiveLearningLoop(dataset,
-get_probabilities=model.predict_on_dataset, heuristic=heuristics.BALD
-(shuffle_prop=0.1), query_size=NDATA_TO_LABEL) for al_step in range(N_ALSTEP):
-model.train_on_dataset(dataset, optimizer, BATCH_SIZE, use_cuda=use_cuda) if
-not active_loop.step(): # We're done! break ``` For a complete experiment, we
-provide _[experiments/](experiments/)_ to understand how to write an active
-training process. Generally, we use the **ActiveLearningLoop** provided at _
-[src/baal/active/active_loop.py](baal/active/active_loop.py)_. This class
-provides functionality to get the predictions on the unlabeled pool after each
-(few) epoch(s) and sort the next set of data items to be labeled based on the
-calculated uncertainty of the pool. ### Re-run our Experiments ```bash docker
-build [--target base_baal] -t baal . docker run --rm baal --gpus all python3
-experiments/vgg_mcdropout_cifar10.py ``` ### Use Baal for YOUR Experiments
-Simply clone the repo, and create your own experiment script similar to the
-example at [experiments/vgg_experiment.py](experiments/vgg_experiment.py). Make
-sure to use the four main parts of Baal framework. _Happy running experiments_
-### Contributing! To contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md). ###
-Who We Are! "There is passion, yet peace; serenity, yet emotion; chaos, yet
-order." The Baal team tests and implements the most recent papers on
-uncertainty estimation and active learning. Current maintainers: - [Parmida
-Atighehchian](mailto:patighehchian@twitter.com) - [FrÃ©dÃ©ric Branchaud-
-Charron](mailto:frederic.branchaud-charron@gmail.com) - [George Pearse]
-(georgehwp26@gmail.com) ### How to cite If you used Baal in one of your
-project, we would greatly appreciate if you cite this library using this
-Bibtex: ``` @misc{atighehchian2019baal, title={Baal, a bayesian active learning
-library}, author={Atighehchian, Parmida and Branchaud-Charron, Frederic and
-Freyberg, Jan and Pardinas, Rafael and Schell, Lorne and Pearse, George}, year=
-{2022}, howpublished={\url{https://github.com/baal-org/baal/}}, } ``` ###
-Licence To get information on licence of this API please read [LICENCE](./
-LICENSE)
+get_probabilities=model.predict_on_dataset, heuristic=heuristics.BALD(),
+iterations=20, # Number of MC sampling. query_size=QUERY_SIZE) # Number of item
+to label. for al_step in range(N_ALSTEP): model.train_on_dataset(dataset,
+optimizer, BATCH_SIZE, use_cuda=use_cuda) metrics = model.test_on_dataset
+(test_dataset, BATCH_SIZE) # Label the next most uncertain items. if not
+active_loop.step(): # We're done! break ``` For a complete experiment, see _
+[experiments/vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_ .
+### Re-run our Experiments ```bash docker build [--target base_baal] -t baal .
+docker run --rm baal --gpus all python3 experiments/vgg_mcdropout_cifar10.py
+``` ### Use Baal for YOUR Experiments Simply clone the repo, and create your
+own experiment script similar to the example at _[experiments/
+vgg_mcdropout_cifar10.py](experiments/vgg_mcdropout_cifar10.py)_. Make sure to
+use the four main parts of Baal framework. _Happy running experiments_ ###
+Contributing! To contribute, see [CONTRIBUTING.md](./CONTRIBUTING.md). ### Who
+We Are! "There is passion, yet peace; serenity, yet emotion; chaos, yet order."
+The Baal team tests and implements the most recent papers on uncertainty
+estimation and active learning. Current maintainers: - [Parmida Atighehchian]
+(mailto:patighehchian@twitter.com) - [FrÃ©dÃ©ric Branchaud-Charron](mailto:
+frederic.branchaud-charron@gmail.com) - [George Pearse](georgehwp26@gmail.com)
+### How to cite If you used Baal in one of your project, we would greatly
+appreciate if you cite this library using this Bibtex: ``` @misc
+{atighehchian2019baal, title={Baal, a bayesian active learning library},
+author={Atighehchian, Parmida and Branchaud-Charron, Frederic and Freyberg, Jan
+and Pardinas, Rafael and Schell, Lorne and Pearse, George}, year={2022},
+howpublished={\url{https://github.com/baal-org/baal/}}, } ``` ### Licence To
+get information on licence of this API please read [LICENCE](./LICENSE)
```

